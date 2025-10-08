<details>
<summary>ENG (English Version)</summary>

# Chapter 12. Advanced Pointers, Dynamic Memory Allocation, and Pointer Arrays in C

## Pointers and Arrays

- A pointer is a variable that stores the memory address of another variable.
- When you declare an array (e.g., `int aa[5];`), the array name (`aa`) itself acts as a constant pointer to its first element.
- You can use a pointer variable (e.g., `int *p;`) to point to the array and access its elements using pointer arithmetic (`*(p + i)` is equivalent to `aa[i]`).
- This allows for flexible and efficient data processing, such as summing all elements of an array using a loop and pointer arithmetic.

## The Need for Dynamic Memory Allocation

- Declaring large arrays statically (e.g., `int aa[10000];`) can waste memory if only a few elements are used.
- Conversely, if more elements are needed than allocated, the program cannot handle additional data.
- Dynamic memory allocation functions allow requesting memory at runtime, allocating exactly the needed amount.

## Dynamic Memory Allocation Functions

- **malloc()**: Allocates a specified amount of memory and returns a pointer to it. The memory is uninitialized.  
  Usage: `p = (int*) malloc(sizeof(int) * cnt);`
- **calloc()**: Similar to `malloc()` but initializes all allocated memory to zero.  
  Usage: `p = (int*) calloc(cnt, sizeof(int));`
- **realloc()**: Changes the size of previously allocated memory (expands or shrinks as needed).  
  Usage: `p = (int*) realloc(p, sizeof(int) * new_size);`
- **free()**: Releases previously allocated memory, returning it to the operating system.  
  Usage: `free(p);`
- Always release dynamically allocated memory with `free()` to avoid memory leaks.

## Pointer Arrays

- A pointer array is an array whose elements are pointers (e.g., `char* p[10];`).
- Useful for handling multiple strings of varying lengths, as each pointer can point to a dynamically allocated memory block sized for each string.
- This approach avoids the memory waste of fixed-size two-dimensional arrays for strings.
- Pointer arrays can also be used with integers or other data types, providing flexibility for dynamic data structures.

</details>

<details>
<summary>KOR (한국어 버전)</summary>

# 12장. 고급 포인터, 동적 메모리 할당, 포인터 배열

## 포인터와 배열

- 포인터는 다른 변수의 메모리 주소를 저장하는 변수임.
- 배열을 선언하면(예: `int aa[5];`) 배열 이름(`aa`) 자체가 첫 번째 요소를 가리키는 상수 포인터 역할을 함.
- 포인터 변수(예: `int *p;`)를 사용해 배열을 가리키고, 포인터 산술 연산(`*(p + i)`)으로 배열 요소에 접근할 수 있음(`aa[i]`와 동일).
- 이를 통해 반복문과 포인터 산술을 이용해 배열 요소 합산 등 유연하고 효율적인 데이터 처리가 가능함.

## 동적 메모리 할당의 필요성

- 큰 배열을 정적으로 선언하면(예: `int aa[10000];`) 일부만 사용할 경우 메모리 낭비가 발생함.
- 반대로 필요한 요소 수보다 적게 할당하면 추가 데이터를 처리할 수 없음.
- 동적 메모리 할당 함수는 실행 중 필요한 만큼 메모리를 요청해 정확한 크기를 할당할 수 있게 함.

## 동적 메모리 할당 함수

- **malloc()**: 지정한 크기만큼 메모리를 할당하고 포인터를 반환함. 메모리는 초기화되지 않음.  
  사용법: `p = (int*) malloc(sizeof(int) * cnt);`
- **calloc()**: malloc과 유사하지만 할당된 메모리를 0으로 초기화함.  
  사용법: `p = (int*) calloc(cnt, sizeof(int));`
- **realloc()**: 이미 할당된 메모리 크기를 변경함(확장 또는 축소).  
  사용법: `p = (int*) realloc(p, sizeof(int) * new_size);`
- **free()**: 할당된 메모리를 해제해 운영체제에 반환함.  
  사용법: `free(p);`
- 메모리 누수를 방지하려면 동적 할당한 메모리는 반드시 `free()`로 해제해야 함.

## 포인터 배열

- 포인터 배열은 요소가 포인터인 배열임(예: `char* p[10];`).
- 길이가 다른 여러 문자열을 다룰 때 유용하며, 각 포인터가 각 문자열에 맞는 동적 메모리를 가리킴.
- 고정 크기 2차원 배열보다 메모리 낭비를 줄일 수 있음.
- 정수 등 다른 데이터 타입에도 포인터 배열을 사용해 동적 데이터 구조를 유연하게 구현할 수 있음.

</details>
