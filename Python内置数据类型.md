## Python内置数据类型

### 容器序列

list、tuple和collection.deque这些序列能存放不同类型的数据，容器序列中存放的是它们所包含的任意类型的对象的引用。

### 扁平序列

str、 bytes、bytearray、memoryview和array.array，这类序列只能容纳一种数据类型。扁平序列里存放的是值而不是引用，即扁平序列存放的是一段连续的内存空间，所以这种序列存储更紧凑，查询速度更快。

### 可变序列

list、bytearray、array.array、collections.deque和memoryview。  

###不可变序列 

tuple、str和bytes

可变序列和不可变序列的差异在于前者在后者的基础上新增一些功能。虽然内置的序列类型并不是直接Sequence和MutableSequence 这两个抽象基类（ Abstract Base Class，ABC）继承而来，但是这些基类可以帮助我们总结出那些完整的序列类型包含了哪些功能。

【超类在左边，子类指向超类】