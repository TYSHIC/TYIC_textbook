# 第一個C++程式

```cpp
#include<iostream>

using namespace std;

int main(){
    cout << "Hello World!" << endl;
    return 0;
}
```

C++和C語言的程式碼有很大的相似之處，但卻又有著許多不同之處。

## 第1行

```cpp
#include<iostream>
```

在C++中，我們不再使用`printf`函式，而是使用`cout`[物件](../advanced/class.md)，
所以不需要引入`stdio.h`標頭檔，而是引入`iostream`標頭檔。

## 第3行

```cpp
using namespace std;
```

`using namespace std;`是用來引入`std`[命名空間](../advanced/namespace.md)，
讓我們可以直接使用`std`命名空間中的內容。

## 第4行

```cpp
cout << "Hello World!" << endl;
```

`cout`是[標準輸出流](../../c/advanced/stream.md)，用來在主控台中輸出文字。

`<<`是[串接運算子](../../c/basic/operator.md)，使資料流入或流出串流。

`"Hello World!"`是字串常數，在這裡被串接運算子流入標準輸出流。

`endl`表示換行。
