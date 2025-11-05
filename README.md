# C

## Variables
A variable is a container that holds data which can be changed during program execution.
1. Variable only start with alphabets or _ (underscore).
2. Variable in case-sensitive 
3. Reserved keyword not allowed in variable name
4. Variable not start with digit
5. Variable should be meaningful
6. Special charactars not allowed in variable name



## Data Type

## 📌 C Language Data Types

| Data Type       | Description                                   | Size (Typical)        | Format Specifier | Example                           |
|-----------------|-----------------------------------------------|-----------------------|------------------|-----------------------------------|
| int             | Integer (whole number)                        | 2 or 4 bytes          | `%d`             | `int a = 10;`                     |
| short           | Smaller integer                               | 2 bytes               | `%hd`            | `short b = 5;`                    |
| long            | Larger integer                                | 4 or 8 bytes          | `%ld`            | `long c = 100000;`                |
| long long       | Very large integer                            | 8 bytes               | `%lld`           | `long long d = 1000000000LL;`     |
| unsigned int    | Only positive integer                         | 2 or 4 bytes          | `%u`             | `unsigned int e = 25;`            |
| float           | Single-precision floating number              | 4 bytes               | `%f`             | `float f = 3.14f;`                |
| double          | Double-precision floating number              | 8 bytes               | `%lf`            | `double g = 3.14159;`             |
| long double     | Extended precision floating number            | 10 or 12 bytes        | `%Lf`            | `long double h = 2.718281828459;` |
| char            | Single character                              | 1 byte                | `%c`             | `char i = 'A';`                   |
| unsigned char   | 0 to 255 character                            | 1 byte                | `%c`             | `unsigned char j = 'B';`          |
| signed char     | -128 to 127 character                         | 1 byte                | `%c`             | `signed char k = 'C';`            |
| void            | No value or empty type                        | —                     | —                | `void func();`                    |
| pointer         | Stores memory address of variable             | 4 or 8 bytes          | `%p`             | `int *ptr = &a;`                  |
---


### ✅ 1. Primary (Built-in) Data Types

| Data Type      | Keyword      | Size (Typical) | Range / Description                                              | Format Specifier | Example        |
|---------------:|-------------:|---------------:|-----------------------------------------------------------------:|-----------------:|---------------:|
| Integer        | `int`        | 2 or 4 bytes   | -32,768 to 32,767 (2B) -2,147,483,648 to 2,147,483,647 (4B)      | `%d`             | `10`           |
| Character      | `char`       | 1 byte         | -128 to 127 (signed) <br> 0 to 255 (unsigned)                    | `%c`             | `'A'`          |
| Floating Point | `float`      | 4 bytes        | ~6 decimal digits precision                                      | `%f`             | `3.14`         |
| Double         | `double`     | 8 bytes        | ~15 decimal digits precision                                     | `%lf`            | `3.1415926535` |
| Void           | `void`       | 0 bytes        | No value / empty                                                 |                  |                |

---

### ✅ 2. Type Modifiers

| Modified Type       | Keyword              | Size (Typical) | Range                                        | Format Specifier | Example      |
|--------------------:|---------------------:|---------------:|---------------------------------------------:|-----------------:|-------------:|
| Short Integer       | `short int`          | 2 bytes        | -32,768 to 32,767                            | `%hd`            | `100`        |
| Long Integer        | `long int`           | 4 or 8 bytes   | -2,147,483,648 to 2,147,483,647              | `%ld`            | `25000`      |
| Long Long Integer   | `long long int`      | 8 bytes        | -(2^63) to (2^63)-1                          | `%lld`           | `9876543210` |
| Unsigned Integer    | `unsigned int`       | 2 or 4 bytes   | 0 to 65,535 (2B) 0 to 4,294,967,295 (4B)     | `%u`             | `50000`      |
| Unsigned Char       | `unsigned char`      | 1 byte         | 0 to 255                                     | `%c`             | `65`         |
| Long Double         | `long double`        | 10/12 bytes    | Higher precision than double                 | `%Lf`            | `3.14159L`   |

---

### ✅ 3. Derived Data Types

| Data Type | Description                                     | Example                                         |
|----------:|------------------------------------------------:|------------------------------------------------:|
| Array     | Collection of same data type                    | `int a[5];`                                     |
| Pointer   | Stores address of a variable                    | `int *p;`                                       |
| Structure | Group of different datatypes                    | `struct student { int id; char name[20]; };`    |
| Union     | Shared memory storage for different data types  | `union data { int x; float y; };`               |
| Enum      | User-defined constants list                     | `enum week {Mon, Tue, Wed};`                    |
| Function  | Block of reusable code                          | `int add(int a, int b);`                        |

---

### ✅ 4. Boolean Support in C (via `<stdbool.h>`)

| Type          | Keyword | Size   | Value            | Example                 |
|--------------:|---------|-------:|-----------------:|------------------------:|
| Boolean       | `bool`  | 1 byte | `true` / `false` | `bool isReady = true;`  |

---

🔔 **Note:** Size of data types may vary on compiler and architecture (32-bit vs 64-bit).  
