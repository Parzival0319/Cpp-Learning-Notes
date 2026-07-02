# 字符串拷贝 strcpy 
## 用于字符串赋值
//char author[40];
  char title[40];
```cpp
strcpy(title, "NULL");
strcpy(author, "NONE");
```

# const
## const 表示参数只读，函数内部不能修改传入的字符串，保证安全、规范、不报错。
` Book(const char t[], const char a[], double p) ` 

# char指针
## 返回字符串 → 必须用 char 指针
## 返回一个数字 → 不用指针，直接 double /int*
```cpp
char* GetTitle() {
    return title;
}
```

# 逗号运算符
## 形式：(表达式1, 表达式2, ... , 表达式n)
## 执行顺序：从左到右依次执行每个表达式。
## 返回值：整个逗号表达式的值是最后一个表达式的值。
```cpp
CDate(int y, int m, int d, int h, int mi, int s): CTime( (cout << "LOVE" << endl, h), mi, s ) { //逗号运算符只能传递一个值
        year = y; month = m; day = d;
}
```

# this 指针
##  指向当前对象自己的指针（成员函数自带，友元函数没有）
## 核心作用
### 1. 解决成员变量和参数重名
```cpp
void setAge(int age) {
    this->age = age;
}
```
### 2. 返回对象自己
```cpp
Student& getSelf() {
    return *this; //链式调用常用
}
```
### 3. 指向当前对象的地址
` cout << this; // 输出对象地址 `

# strcmp
头文件`：#include <cstring>`
## 功能：按字典序比较两个 C 风格字符串，逐位对比 ASCII 码。
##  返回值规则:
```cpp
设两个字符串从左到右第一个不相等字符为 c1、c2
strcmp(s1, s2) > 0：s1 字典序更大（c1 ASCII > c2）
strcmp(s1, s2) == 0：两个字符串完全一模一样
strcmp(s1, s2) < 0：s1 字典序更小（c1 ASCII < c2）
```
