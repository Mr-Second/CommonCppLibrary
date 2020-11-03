# CommonCppLibrary ![](https://img.shields.io/badge/license-MIT-blue) ![](https://img.shields.io/badge/version-C%2B%2B11-brightgreen) ![](https://img.shields.io/badge/version-C%2B%2B14-brightgreen)![](https://img.shields.io/badge/version-C%2B%2B17-brightgreen)![](https://img.shields.io/badge/circleci-passing-brightgreen)

![](https://th.bing.com/th/id/OIP.EQ4hcb5qSYATvd-mOCTFjwHaFj?pid=Api&rs=1)

CommonCppLibrary是一个介绍常见的、有用的和好玩的Cpp库的项目，它具有以下特点
+ 现代： 大部分的库的cpp代码使用的是C++11、C++14以及C++17
+ 实用： 有些库就几个头文件，可以很好的嵌入到你的项目中去
+ 有趣：  C++作为一门比较古老的语言，很多人拿他来做系统底层驱动或者是服务器后台但很少有人用它做一些小工具，而本项目就满足了这些需求.

## Installation
```shell
git clone git@github.com:Mr-Second/CommonCppLibrary.git
```
## Examples
**[PPrinter](https://github.com/Mr-Second/pprint)**

> Pretty Printer for Modern C++

```cpp
#include "pprint.hpp"
#include <iostream>
#include <map>
using namespace std;

int main(int argc, char const *argv[])
{
    pprint::PrettyPrinter printer(cout);
    map<string, int> m;
    m["Today"] = 1;
    m["Tomorrow"] = 2;
    printer.print(m);
    return 0;
}
```

**output**

```
{
Today : 1, 
Tomorrow : 2
}
```

## License
CommonCppLibrary is MIT licensed.