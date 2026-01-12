---
title: "测试四，目录功能TOC"
date: 2026-01-03
summary: "把重复逻辑抽出为可复用模块。"
tags: ["工程", "代码"]
---
减少偶发 bug 的最好办法，是减少重复。
## 1，C语言代码实现Hello World
```c
#include <stdio.h> 
int    main() {
    printf("Hello, World!");
    return 0;
}    
```
### (1),代码说明
- `#include <stdio.h>`：包含标准输入输出库头文件，提供 `printf` 函数的声明。
- `int main()`：定义主函数，程序的入口点，返回类型为整数。
- `printf("Hello, World!");`：调用 `printf` 函数，向标准输出打印字符串 "Hello, World!"。
- `return 0;`：表示程序成功结束，返回值为 0。
- `}`：结束主函数的定义。
### (2),编译与运行
#### 1. 将代码保存到一个名为 `hello.c` 的文件中。
#### 2. 打开终端或命令行界面，导航到保存 `hello.c
#### 3. 文件的目录。
#### 4. 使用 C 编译器（如 `gcc`）编译代码，运行以下命令：
   ```bash
   gcc hello.c -o hello
   ```
#### 5. 编译成功后，运行生成的可执行文件：
   ```bash
   ./hello
   ```
#### 6. 你应该会在终端中看到输出：
   ```Hello, World!
``` 

## 2，C++语言代码实现Hello World
```cpp
#include <iostream>
int main() {
    std::cout << "Hello, World!" << std::endl;
    return 0;
}    
``` 

## 3，Python语言代码实现Hello World
```python
print("Hello, World!")
```

## 4，Java语言代码实现Hello World
```java
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
    }
}
```

## 5，JavaScript语言代码实现Hello World        
```javascript
console.log("Hello, World!");
```

## 6，Go语言代码实现Hello World
```go
package main
import "fmt"
func main() {
    fmt.Println("Hello, World!")
}    
```

## 7，Rust语言代码实现Hello World
```rust
fn main() {
    println!("Hello, World!");
}
```

## 8，Ruby语言代码实现Hello World
```ruby
puts "Hello, World!"
```

## 9，PHP语言代码实现Hello World
```php
<?php
echo "Hello, World!";
?>
```

## 10,8086汇编语言代码实现Hello World
```asm
section .data
    msg db 'Hello, World!',0Ah
    len equ $ - msg
section    .text 
    global _start
_start:
    mov eax, 4
    mov ebx, 1
    mov ecx, msg
    mov edx, len
    int 0x80
    mov eax, 1
    xor ebx, ebx
    int 0x80
```