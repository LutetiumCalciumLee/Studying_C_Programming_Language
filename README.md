<details>
<summary>ENG (English Version)</summary>

# Chapter 11. Input and Output in C

C provides a rich set of functions for handling input and output operations, both for interacting with users (keyboard/screen) and for working with files. All standard I/O functions are defined in the `stdio.h` header.

## Standard Input and Output
- **Standard Input (stdin):** Usually the keyboard.
- **Standard Output (stdout):** Usually the screen.
- **Standard Error (stderr):** Used for error messages, also displayed on the screen.

These are treated as files in C, so input/output operations use the same mechanisms as file operations.

## Types of Input and Output Functions

### Unformatted I/O Functions
- **Character I/O:**  
  - `getchar()` reads a single character from stdin.
  - `putchar()` writes a single character to stdout.
- **String I/O:**  
  - `gets()` reads a line from stdin into a string (deprecated due to safety issues).
  - `puts()` writes a string to stdout.

### Formatted I/O Functions
- **`scanf()`**: Reads formatted input from stdin. Uses format specifiers like `%d`, `%f`, `%s` to read integers, floats, strings, etc.
- **`printf()`**: Writes formatted output to stdout. Uses the same format specifiers to display data in a structured way.

### Safe Alternatives
- **`fgets()`**: A safer alternative to `gets()`, reads a line from stdin with bounds checking.

## Format Specifiers

Format specifiers are used in `scanf()` and `printf()` to indicate the type of data being read or written. Common specifiers include:
- `%d` for integers
- `%f` for floats
- `%c` for characters
- `%s` for strings
- `%lf` for doubles
- `%x` for hexadecimal
- `%o` for octal
- `%p` for pointers

Modifiers can be used for width, precision, and alignment.

## File Input and Output

C treats files as streams of bytes, and all file operations are performed using pointers of type `FILE *`. Key functions include:
- **Opening/Closing Files:**  
  - `fopen()` opens a file for reading, writing, or appending.
  - `fclose()` closes a file.
- **Reading/Writing Files:**  
  - `fgetc()` and `fputc()` read/write single characters.
  - `fgets()` and `fputs()` read/write strings.
  - `fread()` and `fwrite()` read/write blocks of data (often used for binary files).
  - `fprintf()` and `fscanf()` perform formatted I/O with files, similar to `printf()` and `scanf()`.

## Practical Notes
- Always check the result of file operations (e.g., `fopen()`) to avoid errors.
- Use `fgets()` instead of `gets()` for safer string input.
- Understand the difference between formatted and unformatted I/O, and choose the appropriate function for your needs.
- All I/O in C is ultimately stream-based, which makes it flexible but requires careful handling of data types and buffers.

</details>

<details>
<summary>KOR (한국어 버전)</summary>

# 11장. C의 입출력

C 언어는 사용자(키보드/화면)와 파일을 다루는 다양한 입출력 함수를 제공함. 모든 표준 입출력 함수는 `stdio.h` 헤더에 정의되어 있음.

## 표준 입출력
- **표준 입력(stdin):** 일반적으로 키보드임.
- **표준 출력(stdout):** 일반적으로 화면임.
- **표준 에러(stderr):** 오류 메시지 출력에 사용되며, 화면에 표시됨.

이들은 C에서 파일처럼 취급되므로, 입출력 연산은 파일 연산과 동일한 방식으로 처리됨.

## 입출력 함수의 종류

### 비형식 입출력 함수
- **문자 입출력:**  
  - `getchar()`는 표준 입력에서 한 문자를 읽는 함수임.
  - `putchar()`는 표준 출력에 한 문자를 쓰는 함수임.
- **문자열 입출력:**  
  - `gets()`는 표준 입력에서 한 줄을 문자열로 읽는 함수이나, 안전성 문제로 사용이 권장되지 않음.
  - `puts()`는 문자열을 표준 출력에 쓰는 함수임.

### 형식 입출력 함수
- **`scanf()`**: 표준 입력에서 형식화된 데이터를 읽는 함수임. `%d`, `%f`, `%s` 등 서식 지정자를 사용해 정수, 실수, 문자열 등을 입력받음.
- **`printf()`**: 표준 출력에 형식화된 데이터를 출력하는 함수임. 동일한 서식 지정자를 사용해 데이터를 구조적으로 출력함.

### 안전한 대안 함수
- **`fgets()`**: `gets()`보다 안전하게 문자열을 입력받는 함수로, 입력 크기 제한을 설정할 수 있음.

## 서식 지정자

서식 지정자는 `scanf()`와 `printf()`에서 데이터의 타입을 지정하는 데 사용됨. 주요 서식 지정자는 다음과 같음:
- `%d`: 정수
- `%f`: 실수
- `%c`: 문자
- `%s`: 문자열
- `%lf`: double형 실수
- `%x`: 16진수
- `%o`: 8진수
- `%p`: 포인터

너비, 소수점 자리수, 정렬 등 다양한 옵션을 추가할 수 있음.

## 파일 입출력

C 언어는 파일을 바이트 스트림으로 처리하며, 모든 파일 연산은 `FILE *` 타입의 포인터로 수행함. 주요 함수는 다음과 같음:
- **파일 열기/닫기:**  
  - `fopen()`은 파일을 읽기, 쓰기, 추가 모드로 여는 함수임.
  - `fclose()`는 파일을 닫는 함수임.
- **파일 읽기/쓰기:**  
  - `fgetc()`, `fputc()`는 한 문자씩 읽거나 쓰는 함수임.
  - `fgets()`, `fputs()`는 문자열을 읽거나 쓰는 함수임.
  - `fread()`, `fwrite()`는 데이터 블록을 읽거나 쓰는 함수로, 주로 바이너리 파일에 사용됨.
  - `fprintf()`, `fscanf()`는 파일에서 형식화된 입출력을 수행하는 함수로, `printf()`와 `scanf()`와 유사함.

## 실용적 참고 사항
- 파일 연산 결과(예: `fopen()`)를 반드시 확인해 오류를 방지해야 함.
- 문자열 입력에는 `gets()` 대신 `fgets()` 사용이 안전함.
- 형식 입출력과 비형식 입출력의 차이를 이해하고, 목적에 맞는 함수를 선택해야 함.
- C의 모든 입출력은 스트림 기반으로 처리되므로, 데이터 타입과 버퍼 관리에 주의가 필요함.

</details>
