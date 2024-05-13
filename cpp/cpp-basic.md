# CPP Introduciton

## Statement

Statement ialah Unit independen terkecil dari komputasi di CPP dan menjadi instruksi yang paling umum di CPP. Sebagian besar statement di CPP akan diakhiri dengan semicolon (;). Jenis-jenis statements,

- Declaration statements
- Jump statements
- Expression statements
- Compound statements
- Selection statements (conditionals)
- Iteration statements (loops)
- Try blocks

## Function

Statement biasanya dibuat dalam group unit yang disebut function (fungsi). Statement didalam group biasanya dieksekusi secara sequential dari atas ke bawah.

```cpp
// Contoh sebuah Function
int functioncpp()
{
    // Statement here
}
```

## Main Function

Setiap Cpp program harus mempunyai satu spesial function yang bernama __main__. Ketika program berjalan, system akan menjalankan setiap statement di-function main secara sequential.

```cpp
#include <iostream>

// Main function
int main()
{
   std::cout << "Hello world!";
   return 0;
}
```

## Comment
Comment merupakan baris code yang tidak akan dijalankan. Kita dapat menambahkna comment untuk menjelaskan sesuatu dari code.

```cpp
// Ini adalah comment

/* Multiline comment
 * Line 2
 * Line 3
 */
```

## Object and Variables

Proses komputasi merupakan proses manipulasi value. Value bisa apa saja dari data di memory, database, data di jaringan dan lain sebagainya. Didalam cpp, sebenarnya kita tidak diizinkan langsung memanipulasi data di-memory, melainkan kita akan memanipulasi data melalui sebuah object. Misalkan kita definisikan sebuah object untuk menyimpan data phi (3,14). Kita tidak peduli object tersebut dimana disimpan di-memory, tapi kita dapat menggunakannya. Kita dapat memberi nama object tersebut misalnya namanya `nilai_phi` dengan nilai `3.14`. Object yang diberi nama disebut __variable__.

Variabel dalam cpp harus didefinisikan type-nya.

```cpp
// variable x dengan type data int
int;
```