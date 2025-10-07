<details>
<summary>ENG (English Version)</summary>

# Chapter 2. Writing a Simple C Program

## 1. Program Creation Steps
- Create a new project in Visual Studio:  
  [Create New Project] → [C++] → [Windows Desktop Wizard] → Set project name and location → Select 'Empty Project'
- After project creation, add a new C file (.c) to the [Source Files] folder.

## 2. Coding the Program
- Example: Write code to perform addition, subtraction, multiplication, and division on two numbers (100 and 50).
- Declare variables `a`, `b`, and `result`, and print each operation’s result using `printf`.

## 3. Build (Compile/Link)
- Select [Build] → [Build Solution].  
  If there are no errors, the build succeeds; if there are errors, fix the source code and rebuild.

## 4. Run the Program
- Press [Ctrl] + [F5] to run the program.  
  The result is displayed, and pressing any key closes the window.

## 5. Variables vs. Containers
- Variables are storage spaces that retain values during program execution.

---

## Introduction to scanf() Function

### 1. Using Input Functions
- Use `scanf()` or the more secure `scanf_s()` recommended in Visual Studio.  
  (`scanf_s` is only supported in Visual C++.)

### 2. Performing Operations with User Input
- Example: Use `scanf` to input two numbers and print their sum.  
- Use `printf` to display prompts so the user knows what to enter.

</details>

<details>
<summary>KOR (한국어 버전)</summary>

# 2장. 간단한 C 프로그램 작성하기

## 1. 프로그램 생성 단계
- Visual Studio에서 새 프로젝트 생성:  
  [새 프로젝트 만들기] → [C++] → [Windows 데스크톱 마법사] → 프로젝트 이름과 위치 설정 → '빈 프로젝트' 선택  
- 프로젝트 생성 후 [소스 파일] 폴더에 새 C 파일(.c) 추가

## 2. 프로그램 작성
- 예시: 두 숫자(100과 50)에 대한 덧셈, 뺄셈, 곱셈, 나눗셈 연산 코드 작성  
- 변수 `a`, `b`, `result`를 선언하고 `printf`로 각 연산 결과 출력

## 3. 빌드(컴파일/링크)
- [빌드] → [솔루션 빌드] 선택  
  오류가 없으면 빌드가 성공하고, 오류가 있으면 소스를 수정한 뒤 다시 빌드

## 4. 프로그램 실행
- [Ctrl] + [F5] 키로 프로그램 실행  
  결과가 화면에 표시되며, 아무 키나 누르면 창이 닫힘

## 5. 변수와 저장 공간
- 변수는 프로그램 실행 중 값을 유지하는 저장 공간입니다.

---

## scanf() 함수 소개

### 1. 입력 함수 사용
- `scanf()` 또는 Visual Studio에서 권장하는 보안 강화 버전 `scanf_s()` 사용  
  (`scanf_s`는 Visual C++에서만 지원)

### 2. 사용자 입력으로 연산 수행
- 예시: `scanf`로 두 숫자를 입력받아 합을 출력  
- `printf`로 안내 메시지를 출력하여 사용자가 무엇을 입력해야 하는지 알 수 있도록 함

</details>
