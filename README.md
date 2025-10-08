<details>
<summary>ENG (English Version)</summary>

# Chapter 7. Loop Control in C (while, do-while, break, continue, goto, return)

## 1. **while Loop**
- The `while` loop repeatedly executes a block of code as long as a specified condition remains true.
- Before each iteration, the condition is evaluated. If it is true, the loop body runs; if false, the loop exits.
- This structure is useful when the number of iterations is not known in advance and depends on dynamic conditions.
- Proper increment or update of the loop variable inside the loop is essential to avoid infinite loops.

## 2. **do-while Loop**
- The `do-while` loop is similar to the `while` loop but guarantees that the loop body is executed at least once.
- The loop’s body runs first, and the condition is checked after the execution. If the condition is true, the loop repeats; otherwise, it exits.
- This is useful for menu-driven programs or when user input must be processed at least once regardless of the condition.

## 3. **for Loop Comparison**
- The `for` loop is typically used when the number of iterations is known beforehand.
- You can convert a `for` loop to a `while` loop by moving the initialization before the loop and the increment inside the loop body.

## 4. **Infinite Loops**
- Both `while` and `for` loops can be used to create infinite loops by using conditions that are always true (e.g., `while(1)` or `for(;;)`).
- Infinite loops are often used in programs that require continuous user interaction until a break condition is met.

## 5. **break Statement**
- The `break` statement is used to exit a loop immediately, regardless of the condition.
- It is commonly used with `if` statements inside loops to terminate the loop when a specific condition is met.
- In `switch-case` statements, `break` ends the current case block.

## 6. **continue Statement**
- The `continue` statement skips the rest of the code in the current loop iteration and proceeds to the next iteration.
- It is often used to skip over certain values or conditions within a loop without terminating the entire loop.

## 7. **goto Statement**
- The `goto` statement allows for an unconditional jump to a labeled statement within the same function.
- While it can be used for breaking out of deeply nested loops or for error handling, its use is discouraged as it can make code harder to read and maintain.

## 8. **return Statement**
- The `return` statement ends the execution of a function and returns control to the calling function.
- In the `main()` function, `return 0;` typically signals successful program completion.

</details>

<details>
<summary>KOR (한국어 버전)</summary>

# 7장. C의 반복 제어 (while, do-while, break, continue, goto, return)

## 1. **while문**
- `while`문은 지정한 조건이 참인 동안 코드 블록을 반복 실행합니다.
- 각 반복 전에 조건을 검사하며, 참이면 반복문 본문이 실행되고 거짓이면 반복문이 종료됩니다.
- 반복 횟수를 미리 알 수 없고, 동적인 조건에 따라 반복이 결정될 때 유용합니다.
- 반복문 내부에서 반복 변수의 값을 적절히 변경하지 않으면 무한 반복이 발생할 수 있습니다.

## 2. **do-while문**
- `do-while`문은 `while`문과 유사하지만, 반복문 본문이 최소 한 번은 반드시 실행됩니다.
- 반복문 본문이 먼저 실행되고, 그 후 조건을 검사합니다. 조건이 참이면 반복을 계속하고, 거짓이면 종료합니다.
- 메뉴 기반 프로그램이나 사용자 입력을 최소 한 번 이상 처리해야 할 때 유용합니다.

## 3. **for문과의 비교**
- `for`문은 반복 횟수가 미리 정해져 있을 때 주로 사용됩니다.
- 초기화는 반복문 앞에, 증감은 반복문 내부에 넣으면 `for`문을 `while`문으로 변환할 수 있습니다.

## 4. **무한 반복문**
- `while`과 `for` 모두 항상 참인 조건(`while(1)`, `for(;;)` 등)으로 무한 반복문을 만들 수 있습니다.
- 무한 반복문은 사용자의 특정 입력이나 종료 조건이 나올 때까지 계속 동작하는 프로그램에서 자주 사용됩니다.

## 5. **break문**
- `break`문은 조건과 상관없이 반복문을 즉시 종료합니다.
- 반복문 내부의 `if`문과 함께 사용하여 특정 조건에서 반복을 중단할 수 있습니다.
- `switch-case`문에서도 각 case 블록의 종료에 사용됩니다.

## 6. **continue문**
- `continue`문은 현재 반복의 나머지 코드를 건너뛰고 다음 반복으로 넘어갑니다.
- 반복문 내에서 특정 값이나 조건을 건너뛰고 싶을 때 자주 사용됩니다.

## 7. **goto문**
- `goto`문은 동일 함수 내에서 지정한 레이블로 무조건 이동합니다.
- 중첩 반복문 탈출이나 예외 처리에 사용할 수 있지만, 코드의 가독성과 유지보수성을 해치므로 권장되지 않습니다.

## 8. **return문**
- `return`문은 함수의 실행을 종료하고 호출한 곳으로 제어를 반환합니다.
- `main()` 함수에서 `return 0;`은 프로그램이 정상적으로 종료되었음을 의미합니다.

</details>
