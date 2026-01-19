# hello-cpp
# 1. 프로젝트 생성 방법

1. [MinGW 사이트](https://www.msys2.org/)에서 `MinGW`를 다운로드

2. 디렉터리 생성
```bash
mkdir projects
cd projects
mkdir helloworld
cd helloworld
code .
```

3. `projects\helloworld` 경로에 `helloworld.cpp` 파일 생성(**파일 이름은 상관 없음**)

4. `helloworld.cpp` 파일에 해당 코드 입력
```bash
#include <iostream>
#include <vector>
#include <string>

using namespace std;

int main()
{
    vector<string> msg{"Hello", "C++", "World", "from", "VS Code", "and the C++ extension!"};

    for (const string &word : msg)
    {
        cout << word << " ";
    }
    cout << endl;
}

```
5. 우측 상단의 화살표에서 `Run C/C++ File` 메뉴 선택
6. `C/C++:g++.exe build and debug active file` 선택
7. Terminal에서 결과 확인 