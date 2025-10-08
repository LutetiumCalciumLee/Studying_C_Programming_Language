<details>
<summary>ENG (English Version)</summary>

# Chapter 10. Functions in C

## Understanding Functions
- A **function** in C is like a "magic box" that takes input, processes it, and returns an output.
- C provides built-in functions (like `printf()`) and allows users to define their own.
- Using functions avoids repetitive code. For example, instead of writing the same set of instructions multiple times (like making coffee for each customer), you can call a function to perform the task whenever needed.

## Structure and Use of Functions
- A function typically has:
  - A **name**
  - **Parameters (arguments)**: Inputs to the function
  - **Return value**: The result produced by the function
- Calling a function is like pressing a button on a vending machine: you provide some input (like selecting coffee type), and the function returns the result (the prepared coffee).
- Example: A function `plus(int v1, int v2)` returns the sum of two numbers.

## Local and Global Variables
- **Local variables** are declared inside a function and can only be used within that function.
- **Global variables** are declared outside all functions and can be accessed by any function in the program.
- If a local and global variable have the same name, the local variable takes precedence within its function.

## Function Return Values and Parameters
- Functions can be categorized by whether they return a value or not:
  - **Functions with a return value**: Return a result using the `return` statement and must specify a return type (e.g., `int`, `char`).
  - **Functions without a return value**: Use the `void` return type and do not return anything.
- **Parameters** are used to pass information into functions. There are two main ways to pass parameters:
  - **Call by value**: The function receives a copy of the argument’s value. Changes inside the function do not affect the original variable.
  - **Call by address (reference)**: The function receives the address of the argument, allowing it to modify the original variable.

## Key Benefits of Functions
- **Modularity**: Breaks code into manageable sections.
- **Reusability**: Functions can be called multiple times, reducing code duplication.
- **Readability**: Makes programs easier to read and maintain.
- **Debugging**: Isolates errors to specific functions for easier troubleshooting.

</details>

<details>
<summary>KOR (한국어 버전)</summary>

# 10장. C 함수

## 함수의 이해
- 함수는 입력값을 받아 처리한 뒤 결과값을 반환하는 "기능 상자"로 비유할 수 있음.
- C 언어는 printf()와 같은 내장 함수와 사용자가 직접 정의할 수 있는 함수 기능을 제공함.
- 함수를 사용하면 반복적인 코드를 줄일 수 있으며, 예를 들어 여러 번 같은 작업을 수행할 때마다 함수 호출로 간단하게 처리할 수 있음.

## 함수의 구조와 사용
- 함수는 일반적으로 다음 요소로 구성됨:
  - 이름
  - 매개변수(인자): 함수에 전달하는 입력값
  - 반환값: 함수가 처리 후 돌려주는 결과값
- 함수 호출은 자판기 버튼을 누르는 것과 같으며, 입력값을 제공하면 결과값을 반환함.
- 예시: plus(int v1, int v2) 함수는 두 수의 합을 반환함.

## 지역 변수와 전역 변수
- 지역 변수는 함수 내부에서 선언하며, 해당 함수 내에서만 사용 가능함.
- 전역 변수는 모든 함수 외부에서 선언하며, 프로그램 내 모든 함수에서 접근 가능함.
- 지역 변수와 전역 변수의 이름이 같을 경우, 함수 내부에서는 지역 변수가 우선함.

## 함수의 반환값과 매개변수
- 함수는 반환값의 유무에 따라 구분됨:
  - 반환값이 있는 함수는 return문을 사용하며, 반드시 반환형을 명시함(int, char 등).
  - 반환값이 없는 함수는 void 반환형을 사용하며, 값을 반환하지 않음.
- 매개변수는 함수에 정보를 전달하는 역할을 하며, 전달 방식에는 두 가지가 있음:
  - 값에 의한 호출: 함수가 인자의 값을 복사해 받아 처리함. 함수 내부 변경이 원본 변수에 영향을 주지 않음.
  - 주소에 의한 호출(참조): 함수가 인자의 주소를 받아 처리함. 함수 내부 변경이 원본 변수에 영향을 줄 수 있음.

## 함수의 주요 장점
- 모듈화: 코드를 관리하기 쉬운 단위로 분리함.
- 재사용성: 함수를 여러 번 호출해 코드 중복을 줄일 수 있음.
- 가독성: 프로그램을 읽고 유지보수하기 쉬워짐.
- 디버깅: 오류를 특정 함수로 한정해 쉽게 수정할 수 있음.

</details>
