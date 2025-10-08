<details>
<summary>ENG (English Version)</summary>

# Chapter 6. Basics of Loops and the for Loop in C

- The **for loop** is used to repeat a block of code a specific number of times, especially when the number of repetitions is known in advance.

- **Syntax:**
  ```
  for (initialization; condition; increment/decrement) {
      // statements to execute
  }
  ```
  - **Initialization:** Sets the starting value of the loop variable (runs once at the beginning).
  - **Condition:** The loop continues as long as this condition is true. It is checked before each iteration.
  - **Increment/Decrement:** Updates the loop variable after each iteration (usually increases or decreases the value).

- **Execution Order:**
  1. Initialization is executed once at the start.
  2. The condition is checked; if true, the loop body executes.
  3. After the loop body, the increment/decrement expression runs.
  4. Steps 2 and 3 repeat until the condition is false, then the loop ends.

- **Key Points:**
  - The semicolons (;) in the syntax are essential and must not be omitted.
  - You can omit the initialization, condition, or increment/decrement parts, but at least the semicolons must remain. Omitting the condition creates an infinite loop.
  - The for loop is often used for counting, iterating over arrays, or performing repetitive calculations.
  - Nested for loops (a for loop inside another for loop) are common for handling multi-dimensional data or patterns.
  - The loop variable is usually declared and initialized in the initialization part, and its scope is limited to the loop if declared inside the for statement.
  - If the loop body consists of only one statement, the curly braces `{}` can be omitted.

</details>

<details>
<summary>KOR (한국어 버전)</summary>

# 6장. 반복문의 기초와 C의 for문

- **for문**은 반복 횟수가 미리 정해져 있을 때 코드 블록을 여러 번 실행하는 데 사용됩니다.

- **문법:**
  ```
  for (초기화; 조건; 증감) {
      // 실행할 문장들
  }
  ```
  - **초기화:** 반복 변수의 시작값을 설정하며, 반복문 시작 시 한 번만 실행됩니다.
  - **조건:** 이 조건이 참인 동안 반복이 계속되며, 각 반복 전에 검사합니다.
  - **증감:** 각 반복이 끝날 때마다 반복 변수의 값을 변경합니다(주로 증가 또는 감소).

- **실행 순서:**
  1. 초기화가 한 번 실행됩니다.
  2. 조건을 검사하여 참이면 반복문 본문이 실행됩니다.
  3. 반복문 본문 실행 후 증감식이 수행됩니다.
  4. 조건이 거짓이 될 때까지 2, 3단계를 반복하며, 조건이 거짓이면 반복문이 종료됩니다.

- **주요 포인트:**
  - 문법에서 세미콜론(;)은 반드시 포함되어야 하며 생략하면 안 됩니다.
  - 초기화, 조건, 증감 부분을 생략할 수 있지만, 세미콜론은 반드시 남겨야 합니다. 조건을 생략하면 무한 반복이 됩니다.
  - for문은 주로 카운팅, 배열 순회, 반복 계산 등에 자주 사용됩니다.
  - 중첩 for문(다른 for문 안에 for문을 넣는 것)은 다차원 데이터나 패턴 처리에 흔히 사용됩니다.
  - 반복 변수를 for문 안에서 선언하면 그 범위는 해당 for문 내부로 제한됩니다.
  - 반복문 본문이 한 줄일 경우 중괄호 `{}`는 생략할 수 있습니다.

</details>
