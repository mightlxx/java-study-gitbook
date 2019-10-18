# Java容器基础

## 1. 说说List、Set、Map三者的区别

- List：List接口存储一组不唯一（可以有多个元素引用相同的对象），有序的对象
- Set（注重独一无二的性质）：不允许重复的集合，不会有多个元素引用相同的对象
- Map（用key来搜索的专家）：使用键值对存储。Map会维护与key有关联的值。两个key可以引用相同的对象，但key不能重复。

## 2. ArrayList 和 LinkedList 区别？

1. **是否保证线程安全**：ArrayList 和 LinkedList 都是不同步的，也就是不保证线程安全
2. **底层数据结构**：ArrayList 底层使用的是**Object 数组**，LinkedList 底层使用的是**双向链表**（JDK1.6之前为循环链表，JDK1.7取消了循环）

3. **插入和删除是否受元素位置的影响**：

   |            | ArrayList（数组）                      | LinkedList(链表)         |
   | ---------- | -------------------------------------- | ------------------------ |
   | 是否影响   | 影响                                   | 不影响                   |
   | 算法复杂度 | 追加到末尾O(1)，插入和删除i位置 O(N-1) | 插入删除都不影响都是O(1) |

4. **是否支持随机访问**：LinkedList 不支持高效的随机元素访问，而ArrayList 支持。

   >快速随机访问就是通过元素的序号快速获取元素对象(对应于`get(int index) `方法)。

5. **内存空间占用**：ArrayList 的空间浪费主要体现在list列表的结尾会预留一定的容量空间。而LinkedList 的空间花费则体现在他的每一个元素都需要消耗比ArrayList更多的空间（因为要存放直接后继和直接前驱以及数据）

### 2.1 Linked为什么不支持随机访问(RandomAccess接口)

RandomAccess接口中什么都没有定义，只是一个标识，标识实现这个接口的类具有随机访问的功能

**`ArrayList` 实现了 `RandomAccess` 接口， 而 `LinkedList` 没有实现。为什么呢？**

我觉得还是和底层数据结构有关！`ArrayList` 底层是数组，而 `LinkedList` 底层是链表。数组天然支持随机访问，时间复杂度为 O（1），所以称为快速随机访问。链表需要遍历到特定位置才能访问特定位置的元素，时间复杂度为 O（n），所以不支持快速随机访问。，`ArrayList` 实现了 `RandomAccess` 接口，就表明了他具有快速随机访问功能。 `RandomAccess` 接口只是标识，并不是说 `ArrayList` 实现 `RandomAccess` 接口才具有快速随机访问功能的！

### 2.2 list 遍历方式选择

- 实现了RandomAccess 接口的list，优先选择普通for循环，其次foreach
- 未实现 RandomAccess 接口的list，优先选择iterator遍历（foreach遍历底层也是通过iterator实现），大size的数据，千万不要使用普通for循环

### 2.3 补充：双向链表和双向循环列表

**双向链表**：包含两个指针，一个prev指向前一个节点，一个next指向后一个节点

![image-20191018213436185](/Users/zhangshengzhong/Library/Application Support/typora-user-images/image-20191018213436185.png)

**双向循环链表**：最后一个节点的next指向head，而head 的prev指向最后一个节点，构成一个环

## 3.ArrayList与Vector区别？为什么要用ArrayList取代Vector呢？

Vector 类的所有方法都是同步方法的。可以由两个线程安全得访问一个Vector对象。但是一个线程访问Vector的话代码要在同步操作上耗费大量的时间

ArrayList 不是同步的，所以在不需要保证线程安全时建议使用ArrayList

## 4. ArrayList 的扩容机制

[ArrayList 的扩容机制](./ArrayList 的扩容机制.md)

## 5. HashMap 和 Hashtable 的区别

1. **线程是否安全**：HashMap是非线程安全的，HashTable是线程安全的；HashTable内部的方法基本都经过synchronized修饰。（如果你要保证线程安全的话使用ConcureentHashMap）
2. **效率**：因为线程安全的问题，HashMap 要比HashTable 效率要高一点，另外，HashTable 基本被淘汰，不要再代码中使用它
3. 对Null key 和Null value 的支持：HashMap 中，null 可以作为键，这样的键只有一个，可以有一个或多个键所对应的值为null。。但是在hashTable中put进的键值只要有一个null，直接抛出NullPointerException。
4. 初始容量大小和每次扩充容量大小的不同：
   1. 创建时如果不指定容量初始值。
      1. Hashtable默认的初始大小为11，之后每次扩充，容量变为原来的2n+1
      2. HashMap 默认的初始化大小为16.之后每次扩充，容量变为原来的2倍
   2. 创建时如果给定了容量初始值
      1. Hashtable 会直接使用你给定的大小
      2. HashMap 会将其扩充为2的幂次方大小（也就是说 HashMap 总是使用2的幂作为哈希表的大小,）
5. 底层数据结构：JDK1.8 以后的HashMap 在解决哈希冲突时有了较大的变化。当链表长度大于阈值（默认是8），将链表转为红黑树，以减少搜索时间。HashTable
   没有这样的机制

## 6. HashMap 如何保证总是使用2的幂次方作为哈希表的大小

**HashMap 中带有初始容量的构造函数：**

```java
public HashMap(int initialCapacity, float loadFactor) {
        if (initialCapacity < 0)
            throw new IllegalArgumentException("Illegal initial capacity: " +
                                               initialCapacity);
        if (initialCapacity > MAXIMUM_CAPACITY)
            initialCapacity = MAXIMUM_CAPACITY;
        if (loadFactor <= 0 || Float.isNaN(loadFactor))
            throw new IllegalArgumentException("Illegal load factor: " +
                                               loadFactor);
        this.loadFactor = loadFactor;
        this.threshold = tableSizeFor(initialCapacity);
    }
     public HashMap(int initialCapacity) {
        this(initialCapacity, DEFAULT_LOAD_FACTOR);
    }
```

下面这个方法保证了 HashMap 总是使用2的幂作为哈希表的大小。

```java
 /**
     * Returns a power of two size for the given target capacity.
     */
    static final int tableSizeFor(int cap) {
        int n = cap - 1;
        n |= n >>> 1;
        n |= n >>> 2;
        n |= n >>> 4;
        n |= n >>> 8;
        n |= n >>> 16;
        return (n < 0) ? 1 : (n >= MAXIMUM_CAPACITY) ? MAXIMUM_CAPACITY : n + 1;
    }
```

## 7. HashMap 和 HashSet区别

HashSet 底层就是基于 HashMap 实现的，（HashSet 的源码非常非常少，除了clone()、writeObject()、readObject（）是hashSet自己不得不实现指纹，其他都是调用hashMap中的方法）

| HashMap                         | hashSet                                                      |
| ------------------------------- | ------------------------------------------------------------ |
| 实现了Map接口                   | 实现了set接口                                                |
| 存储键值对                      | 仅存储对象                                                   |
| 调用put() 向map中添加元素       | 调用add 方法向set中添加元素                                  |
| HashMap 使用（key）计算hashcode | HashSet使用成员对象来计算hashcode值，对于两个对象来说hashcode可能相同。所以equals（）方法来判断对象的相等行 |

## 8. HashSet如何检查重复

当你吧对象加入HashSet 时，

- HashSet会先计算对象的hashCode来判断对象加入的位置，
- 同时也会与其他加入的对象的hashCode值做比较。如果没有相符的hashCode，hashSet 会假设对象没有重复出现。
- 但是如果方向有hashCode值的对象，这时候会调用equals（）方法来检查hashCode相等的对象是否真的相同。如果两者相同，hashSet就不会让加入操作成功

### 8.1 **hashCode（）与equals（）的相关规定：**

1. 如果两个对象相等，则hashcode一定也是相同的
2. 两个对象相等,对两个equals方法返回true
3. 两个对象有相同的hashcode值，它们也不一定是相等的
4. 综上，equals方法被覆盖过，则hashCode方法也必须被覆盖
5. hashCode()的默认行为是对堆上的对象产生独特值。如果没有重写hashCode()，则该class的两个对象无论如何都不会相等（即使这两个对象指向相同的数据）。

### 8.2 ==与equals的区别

1. ==是判断两个变量或实例是不是指向同一个内存空间 equals是判断两个变量或实例所指向的内存空间的值是不是相同
2. ==是指对内存地址进行比较 equals()是对字符串的内容进行比较
3. ==指引用是否相同 equals()指的是值是否相同