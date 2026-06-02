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
