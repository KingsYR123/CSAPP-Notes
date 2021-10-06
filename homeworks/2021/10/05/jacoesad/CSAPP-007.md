> ***2021.10.05\***

------

### 2.1.5 Representing Code

从机器角度看，程序仅仅是字节序列。一样的进程，运行在不同操作系统，二进制代码也不会相同。

### 2.1.6 Introduction to Boolean Algebra

布尔代数：通过逻辑值TRUE和FALSE编码为二进制0和1，设计出一种代数，研究逻辑推理的基本过程。

布尔运算VS逻辑运算：

- ~—— NOT：P与~P相反
- &—— AND：当且仅当p=1且q=1时，p&q才等于1
- |—— OR：当p=1或者q=1时，p|q才等于1
- ^—— EXCLUSIVE-OR：当p=1或者q=0，或者p=0或者q=1时，p^q等于1

布尔运算可以扩展到位向量运算，位向量就是固定长度w，由0、1组成的串。位向量的运算即为每个对应元素的运算。

位向量可以作为向量掩码，当某一位上位1时，表示信号是有效的，当是0时表示信号是被屏蔽的。

### 2.1.7 Bit-Level Operations in C

C语言支持按位布尔运算。|或、&与、~取反、^异或。

掩码运算——表示从一个字中选出的位的集合。例如：掩码0xFF表示一个字的低位字节。位运算x&0xFF生成一个由x的最低有效字节组成的值。表达式~0将生成一个全1的掩码，不管机器的字大小是多少。