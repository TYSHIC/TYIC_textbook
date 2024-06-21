# 第一個C語言程式

第一個c語言程式

```c
#include<stdio.h>

int main(){
    printf("Hello World!");
    return 0;
}
```

上面的程式碼可以在主控台(console)中輸出「Hello World!」，讓我們從第一行開始依序看起：

第一行：

```c
#include<stdio.h>
```

在C/C++中，以「#」開頭的程式碼為「[前置處理器](../advanced/preprocessor.md)」。

而「include」則是前置處理器的一種，用來引入[標頭檔](../advanced/header_namespace)。

因為「printf」這個[函式](./function.md)定義在「stdio.h」這個標頭檔中，所以必須引入才可以使用「printf」這個函數。

