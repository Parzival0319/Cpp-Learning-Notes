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

# 指针
## 返回字符串 → 必须用 char 指针
## 返回一个数字 → 不用指针，直接 double /int*
```cpp
char* GetTitle() {
    return title;
}
```
