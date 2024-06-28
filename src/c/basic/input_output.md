# 輸入與輸出

在 C 語言中，我們可以使用 `printf()` 函數來輸出資料、`scanf()` 函數來輸入資料。

## 輸出

`printf` 是用來輸出資料的函式，其[函式原型](./function.md)如下：

```c
int printf(const char *format, ...);
```

`printf` 函式的第一個參參數是一個[字元](./data_type.md)指標，
這個字串可以包含文字格式化符號，例如 `%d`、`%f`、`%s`，
這些格式化符號會被後面的參數取代，
所以對於不同[資料型態](./data_type.md)的參數，必須使用不同的格式化符號。

以下是一些常見的文字格式化符號：

| 格式化符號 | 對應資料型態 |
|:-----:|:------:|
| `%d`  |   整數   |
| `%f`  |  浮點數   |
| `%c`  |   字元   |
| `%s`  |   字串   |

`printf` 函式接著可以接受多個參數，這些參數會依序取代字串中的格式化符號。

以下是一個簡單的範例：

```c
#include<stdio.h>

int main(){
    printf("6 + 8 = %d\n", 6 + 8);
    printf("pi = %f\n", 3.14);
    printf("first letter: %c\n", 'a');
    printf("hello %s\n", "world");

    return 0;
}
```

```
6 + 8 = 14
pi = 3.140000
first letter: a
hello world
```

## 輸入

`scanf` 是用來輸入資料的函式，其函式原型如下：

```c
int scanf(const char *format, ...);
```

`scanf` 函式的第一個參數和 `printf` 函式一樣。