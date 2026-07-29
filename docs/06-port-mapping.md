## 6. 포트 매핑 접속(2회)

---

### 6-1. 두 개의 컨테이너 실행하기

<img width="2648" height="224" alt="image" src="https://github.com/user-attachments/assets/4240faea-0de4-46f7-931e-9c2394451035" />

8080, 8081 포트가 실행 중인 것을 볼 수 있다.

구조는 다음과 같다.  
localhost:8080 → web-test 컨테이너의 80번 포트  
localhost:8081 → web-test-2 컨테이너의 80번 포트

---

### 6-2. 접속 확인

<img width="1404" height="424" alt="image" src="https://github.com/user-attachments/assets/dcc7578e-a337-47fb-b817-136c78daee75" />

첫 번째 컨테이너의 접속을 확인했다.

<img width="1406" height="446" alt="image" src="https://github.com/user-attachments/assets/5edfe8a0-9b86-4522-9b95-8f9b5f218923" />

두 번째 컨테이너의 접속을 확인했다.

---

### 6-3. 포트 충돌 확인하기

<img width="1412" height="330" alt="image" src="https://github.com/user-attachments/assets/9e4e32f8-bf0e-4edc-9f9f-6be4c1fcf2fe" />

web-test가 8080 포트를 사용 중인 상태에서 이 명령어를 실행해보면 오류가 난다.

컨테이너 내부 포트는 같아도 되지만 호스트 포트는 중복되면 안 된다.

---
