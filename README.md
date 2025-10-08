<details>
<summary>ENG (English Version)</summary>

# Chapter 8. Understanding Arrays in C

### What is an Array?
- An array is a way to group multiple variables of the same type under a single name, allowing you to manage and process collections of data efficiently.
- Each element in an array is accessed using an index (subscript), starting from 0. For example, `aa[0]`, `aa[1]`, `aa[2]`, ...

### Why Use Arrays?
- Without arrays, you would need to declare separate variables for each value (e.g., `int a, b, c, d;`).
- Arrays allow you to handle large sets of data with loops, making your code more concise and easier to manage.
- They are especially useful when dealing with repetitive operations, such as storing and processing scores, sensor readings, or any series of related values.

### Declaring and Initializing Arrays
- Arrays are declared by specifying the data type, array name, and the number of elements in square brackets (e.g., `int aa[4];`).
- You can initialize arrays at the time of declaration using braces and commas (e.g., `int aa[4] = {100, 200, 300, 400};`).
- If the number of initial values is less than the array size, the remaining elements are set to 0.
- If you omit the size, the array will automatically be sized to fit the number of initial values (e.g., `int aa[] = {100, 200, 300, 400};`).
- If you declare an array without initializing it, its elements contain garbage values.

### Using Arrays with Loops
- Arrays are most powerful when used with loops, such as `for` loops, to process all elements efficiently.
- For example, you can use a loop to input values into an array, calculate the sum, or print all elements without writing repetitive code for each variable.
- This is especially beneficial for large arrays, as a single loop can process hundreds or thousands of elements.

### Determining Array Size
- The number of elements in an array can be determined using the `sizeof` operator:  
  `number of elements = sizeof(array) / sizeof(element type);`
- This allows you to write flexible code that adapts to arrays of different sizes.

### Arrays and Strings
- Character arrays are used to store strings in C.
- Strings are simply arrays of characters ending with a null character (`'\0'`).
- You can manipulate strings using standard library functions like `strlen()` (to get string length), `strcpy()` (to copy strings), `strcat()` (to concatenate), and `strcmp()` (to compare).
- String input and output can be handled with functions like `gets()` and `puts()`, but safer alternatives like `fgets()` and `puts()` are recommended.

### Multi-dimensional Arrays
- C supports multi-dimensional arrays, such as two-dimensional arrays for matrices or tables (e.g., `int aa[3][4];`).
- Elements are accessed using multiple indices (e.g., `aa[1][2]`).
- Two-dimensional arrays can be initialized with nested braces, and processed using nested loops.
- Higher-dimensional arrays (three or more dimensions) are also supported for more complex data structures.

</details>

<details>
<summary>KOR (한국어 버전)</summary>

# 8장. C 배열 이해하기

### 배열이란?
- 배열은 같은 타입의 여러 변수를 하나의 이름으로 묶어 효율적으로 데이터 집합을 관리 및 처리하는 방법임.
- 배열의 각 요소는 0부터 시작하는 인덱스(첨자)를 사용해 접근함. 예: `aa[0]`, `aa[1]`, `aa[2]` 등.

### 배열을 사용하는 이유
- 배열이 없으면 각각의 값을 위해 별도의 변수를 선언해야 하는 불편함이 있음(예: `int a, b, c, d;`).
- 배열을 사용하면 반복문으로 많은 데이터를 간결하게 처리할 수 있어 코드 관리가 쉬워짐.
- 점수, 센서 데이터 등 반복적인 값의 저장 및 처리에 특히 유용함.

### 배열 선언과 초기화
- 배열은 데이터 타입, 배열 이름, 대괄호 안에 요소 개수를 지정하여 선언함(예: `int aa[4];`).
- 선언과 동시에 중괄호와 쉼표로 초기화할 수 있음(예: `int aa[4] = {100, 200, 300, 400};`).
- 초기값이 배열 크기보다 적으면 나머지 요소는 0으로 자동 초기화됨.
- 크기를 생략하면 초기값 개수에 맞춰 배열 크기가 자동 결정됨(예: `int aa[] = {100, 200, 300, 400};`).
- 초기화 없이 배열을 선언하면 요소에 쓰레기 값이 저장됨.

### 반복문과 배열 사용
- 배열은 `for`문 등 반복문과 함께 사용할 때 모든 요소를 효율적으로 처리할 수 있음.
- 반복문을 이용해 배열에 값 입력, 합계 계산, 전체 요소 출력 등 반복적인 작업을 간단하게 구현할 수 있음.
- 대용량 배열도 한 번의 반복문으로 수백, 수천 개 요소를 처리할 수 있음.

### 배열 크기 구하기
- `sizeof` 연산자를 사용해 배열 요소 개수를 구할 수 있음:  
  `요소 개수 = sizeof(배열) / sizeof(요소 타입);`
- 다양한 크기의 배열에 유연하게 대응하는 코드 작성이 가능함.

### 배열과 문자열
- 문자 배열은 C에서 문자열을 저장하는 데 사용됨.
- 문자열은 널 문자(`'\0'`)로 끝나는 문자 배열임.
- `strlen()`, `strcpy()`, `strcat()`, `strcmp()` 등 표준 라이브러리 함수로 문자열을 다룰 수 있음.
- 문자열 입출력은 `gets()`, `puts()`로 할 수 있으나, `fgets()`와 `puts()` 같은 안전한 함수 사용이 권장됨.

### 다차원 배열
- C는 행렬, 표 등을 위한 2차원 배열 등 다차원 배열을 지원함(예: `int aa[3][4];`).
- 요소는 여러 인덱스를 사용해 접근함(예: `aa[1][2]`).
- 2차원 배열은 중첩 중괄호로 초기화하고, 중첩 반복문으로 처리함.
- 3차원 이상 고차원 배열도 복잡한 데이터 구조에 활용 가능함.

</details>
