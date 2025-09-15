# ✅ Day 1: C++ 기초

---

## 1️⃣ 개념 정리

- **C++ 프로그램 구조**: `main` 함수, 반환값 의미 (`int`)
- **입출력 스트림**: `cout`, `cin` (공백 단위 입력 주의)
- **기본 자료형**: `int`, `double`, `char`, `bool`, `string`
- **auto** 키워드: 타입 자동 추론
- **프로그램 인자**: `argc`, `argv`와 함수 매개변수 비교

---

## 2️⃣ 예제 코드

```cpp
#include <iostream>
#include <string>
using namespace std;

int main(int argc, char* argv[]) {
    int age = 25;
    double height = 175.5;
    char grade = 'A';
    bool isStudent = true;
    string name = "Yong Tae";
    auto score = 95;
    auto pi = 3.14159;

    cout << "이름: " << name << endl;
    cout << "나이: " << age << endl;
    cout << "키: " << height << "cm" << endl;
    cout << "학점: " << grade << endl;
    cout << "학생 여부: " << boolalpha << isStudent << endl;
    cout << "점수: " << score << ", 원주율: " << pi << endl;

    int x;
    cout << "숫자를 입력하세요: ";
    cin >> x;
    cout << "입력한 숫자: " << x << endl;

    cout << "argc = " << argc << endl;
    for (int i = 0; i < argc; i++)
        cout << "argv[" << i << "] = " << argv[i] << endl;

    return 0;
}

```

## 3️⃣ 연습문제

- [ ]  이름, 나이, 좋아하는 숫자를 입력받아 출력
- [ ]  `auto` 키워드로 여러 변수 선언 후 출력
- [ ]  `bool` 변수의 `true/false` 출력 비교 (`boolalpha` 사용)

## 4️⃣ 추가 팁

- `cin`은 공백 단위로 끊어서 입력
- 공백 포함 문자열 입력 시: `getline(cin, str)`
- `argv[0]` 항상 프로그램 이름, 추가 인자부터 `argv[1]`
