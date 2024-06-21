# 第一個C語言程式

```c
#include<stdio.h>

int main(){
    printf("Hello World!");
    return 0;
}
```

在C/C++中，每個陳述句(statement)都必須以分號「;」結尾。

上面的程式碼可以在主控台(console)中輸出`Hello World!`，
讓我們從第一行開始依序看起：

## 第1行

```c
#include<stdio.h>
```

在C/C++中，以「#」開頭的程式碼為[前置處理器](../advanced/preprocessor.md)，
而`include`則是前置處理器的一種，用來引入[標頭檔](../advanced/header_namespace)。

因為`printf`這個[函式](./function.md)定義在`stdio.h`這個標頭檔中，
所以必須引入`stdio.h`這個標頭檔才可以使用`printf`這個函式。

## 第3~6行

```c
int main(){
    printf("Hello World!");
    return 0;
}
```

### 第3、6行

`int main(){}`是定義一個函式，並且是個主函式，程式會從這個函式開始執行。

`int`表示這個函式的[回傳值](./function.md)是一個[整數](./data_type.md)。

`()`是用來放[參數](./function.md)的地方，在這個函式中是空的，表示這個函式沒有參數。

`{}`是一個[區塊](./control_flow.md)，用來包裹要執行的程式碼。

### 第4行

```c
printf("Hello World!");
```

`printf`是一個函式，用來在主控台中[輸出](./input_output.md)文字。

`"Hello World!"`是一個[字串](./string.md)[常數](./variable_constant.md)，
作為[引數](./function.md)傳給`printf`函式，讓其輸出`Hello World!`在主控台中。

### 第5行

```c
return 0;
```

`return`是個關鍵字，其作用是回傳。

`0`是一個整數常數，
通常在`main`函式的回傳值中所代表的意思為「程式執行成功」。

