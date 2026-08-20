<details>
<summary>ENG (English Version)</summary>

# Chapter 3. printf Function and Formatted Input/Output in C

## Overview
- **printf** is a standard C library function used to output formatted text to the screen.
- The function takes a *format string* (which may include plain text and format specifiers starting with `%`) and a variable number of arguments to print.
- Format specifiers, such as `%d` for integers, `%s` for strings, `%f` for floating-point numbers, and `%c` for characters, determine how each value is displayed in the output.
- The format string can also include options for width, precision, and flags to control alignment, padding, and formatting details.
- To use `printf`, include the header file `#include <stdio.h>` at the top of your program.
- The related function `scanf` is used for formatted input, allowing users to enter values in a specified format.
- Advanced formatting options allow for dynamic width and precision using asterisks (`*`) in the format string, with values provided as additional arguments.

</details>

<details>
<summary>KOR (한국어 버전)</summary>

# 3장. printf 함수와 C 언어의 형식화 된 입출력

## 개요
- **printf**는 화면에 형식화된 텍스트를 출력하는 C 표준 라이브러리 함수입니다.
- *서식 문자열* (일반 텍스트와 `%`로 시작하는 형식 지정자를 포함할 수 있음)과 출력할 여러 인자를 전달받아 동작합니다.
- 형식 지정자 `%d`(정수), `%s`(문자열), `%f`(실수), `%c`(문자) 등을 사용해 각 값이 어떻게 출력될지 설정할 수 있습니다.
- 서식 문자열에는 너비, 소수점 자리수, 정렬, 공백 채우기 등 출력을 제어하는 옵션도 포함될 수 있습니다.
- `printf`를 사용하려면 프로그램 상단에 `#include <stdio.h>`를 포함해야 합니다.
- 관련 함수 `scanf`는 형식화된 입력을 수행하며, 지정한 형식에 맞게 값을 입력받을 수 있습니다.
- 고급 형식 옵션으로, 형식 문자열에서 별표(`*`)를 사용하면 너비와 소수점 자리수를 동적으로 지정할 수 있고, 이에 필요한 값은 추가 인자로 제공됩니다.

</details>
