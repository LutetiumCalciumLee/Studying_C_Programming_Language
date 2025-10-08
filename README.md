<details>
<summary>ENG (English Version)</summary>

# Chapter 9. Arrays and Pointers

## 1. Stack

- A **stack** is a data structure where elements are added and removed from only one end, following the Last In, First Out (LIFO) principle.
- The **top** indicates the position of the most recently added data.
- **Push** adds data to the stack, and **pop** removes the most recent data.
- Stacks can be implemented using arrays, with a variable (e.g., `top`) tracking the current position.
- Proper error handling is necessary to prevent pushing onto a full stack or popping from an empty stack.
- Practical stack operations include adding and removing elements, as well as checking the current size.

## 2. Memory and Addresses

- Variables are stored in memory, and each memory location has a unique address.
- The size of a variable (e.g., an `int` is typically 4 bytes) determines how much memory it occupies.
- The address of a variable can be obtained using the `&` operator (e.g., `&a`).
- Arrays are stored in contiguous memory locations. The address of each element can be calculated based on the base address and element size.
- The name of an array represents the address of its first element.

## 3. Pointers

- A **pointer** is a variable that stores the address of another variable.
- Pointers are declared using the `*` symbol (e.g., `int *p;` for an integer pointer).
- Assigning a variable's address to a pointer allows indirect access to the variable's value using the dereference operator `*`.
- The size of a pointer is typically 4 bytes, regardless of the data type it points to.
- Pointers can be used to manipulate data stored in other variables, swap values, and traverse arrays.

## 4. Relationship Between Arrays and Pointers

- The name of an array acts as a pointer to its first element.
- Pointer arithmetic allows navigation through array elements (e.g., `*(array + i)` is equivalent to `array[i]`).
- Pointers and arrays are closely related; pointers can be used to access and manipulate array data efficiently.
- For character arrays (strings), pointers are often used for string manipulation and traversal.
- Examples include reversing a string using pointers, swapping values, and sorting arrays by manipulating elements through pointers.

</details>

<details>
<summary>KOR (한국어 버전)</summary>

# 9장. 배열과 포인터

## 1. 스택

- 스택은 한쪽 끝에서만 데이터를 추가하거나 제거하는 자료구조로, 후입선출(LIFO) 원칙을 따름.
- top은 가장 최근에 추가된 데이터의 위치를 나타내는 변수임.
- push는 데이터를 스택에 추가하는 연산, pop은 가장 최근 데이터를 제거하는 연산임.
- 스택은 배열로 구현할 수 있으며, 현재 위치를 추적하는 top 변수를 사용함.
- 스택이 가득 찼을 때 push, 비어 있을 때 pop을 방지하기 위한 오류 처리가 필요함.
- 스택의 주요 연산은 요소 추가, 제거, 현재 크기 확인임.

## 2. 메모리와 주소

- 변수는 메모리에 저장되며, 각 메모리 위치는 고유한 주소를 가짐.
- 변수의 크기(예: int는 일반적으로 4바이트)는 메모리 점유량을 결정함.
- 변수의 주소는 & 연산자(예: &a)로 확인 가능함.
- 배열은 연속된 메모리 공간에 저장되며, 각 요소의 주소는 시작 주소와 요소 크기로 계산함.
- 배열 이름은 첫 번째 요소의 주소를 나타냄.

## 3. 포인터

- 포인터는 다른 변수의 주소를 저장하는 변수임.
- 포인터는 * 기호를 사용해 선언함(예: int *p;는 int형 포인터임).
- 변수의 주소를 포인터에 대입하면 * 연산자로 해당 변수의 값을 간접적으로 접근할 수 있음.
- 포인터의 크기는 가리키는 데이터 타입과 관계없이 일반적으로 4바이트임.
- 포인터는 다른 변수의 데이터 조작, 값 교환, 배열 순회 등에 활용됨.

## 4. 배열과 포인터의 관계

- 배열 이름은 첫 번째 요소의 주소를 나타내므로 포인터처럼 동작함.
- 포인터 연산을 통해 배열 요소를 탐색할 수 있음(예: *(array + i)는 array[i]와 동일함).
- 포인터와 배열은 밀접한 관계가 있으며, 포인터로 배열 데이터를 효율적으로 접근 및 조작할 수 있음.
- 문자 배열(문자열)에서는 포인터를 활용해 문자열 처리와 탐색을 수행함.
- 포인터를 이용한 문자열 뒤집기, 값 교환, 배열 정렬 등 다양한 예시가 존재함.

</details>
