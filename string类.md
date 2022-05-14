# string类

包含头文件string

位于命名空间std中

```c++
#include<string>
using namespace std;
```

可以使用c风格字符串初始化string对象

```c++
string str1="panther";
string str3 {"列表初始化"};
```

可以使用cin将键盘输入存储到string对象中

```c++
string str2;
cin>>str2;
```

可以用cout来显示string对象

```c++
cout<<str1;
```

可以使用下标运算符 '[]' 访问string对象中的字符

```c++
str2[3]
```

string对象可以自动调整长度，比数组更加安全

## 赋值

可以直接用赋值运算符'='

```c++
string str1,str2;
str1 = str2;
```

c风格的操作

```c++
#include<cstring>
strpy(charr1,charr2);// 拼接charr1 = charr2
```

## 拼接&附加

直接用运算符'+'就能合并两个string对象

还可以用'+='附加字符串

```c++
string str3;
str3 = str1 + str2;
str1 += str2;
str2 += "hello";
```

c风格的操作

```c++
#include<cstring>
strcat(charr1,charr2);//拼接 charr1 += charr2
```

使用字符数组有存在目标数组过小 覆盖相邻内存的风险

而string类会自动调整大小

## 字符串长度

```c++
int len1 = str1.size();//利用成员函数获取长度
```

c风格的操作

```c++
#include<cstring>
int len2 = strlen(charr1);
```

### string类I/O

cin>>存储string对象、cout<<显示string对象

cin读取string对象时每次读取一行 而不是一个

未初始化的数组 空字符位置是随机的

未初始化的string对象字符串长度为0

```c++
getline(cin,str);
此处的getline()不是类方法
将cin作为参数，指出去哪里查找输入
```
