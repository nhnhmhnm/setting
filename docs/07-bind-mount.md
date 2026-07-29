## 7. 바인드 마운트 반영

| 명령어 | 역할 |
| --- | --- |
| docker compose up -d | 실행 |
| docker compose ps | 상태 확인 |
| docker compose logs | 로그 확인 |
| docker compose down | 종료 및 삭제 |
| docker compose restart | 다시 시작 |

---

### 7-1. 바인드 마운트 컨테이너 실행

<img width="1414" height="102" alt="image" src="https://github.com/user-attachments/assets/ecf9a54e-13cf-4d60-880a-23fac809165d" />

8082 포트를 사용해 실행했다.

| 명령어 | 역할 |
| --- | --- |
| --name web-bind-test | 컨테이너 이름 지정 |
| -p 8082:80 | 내 컴퓨터 8082 포트를 컨테이너 80 포트에 연결 |
| -v "$(pwd)/index.html:/usr/share/nginx/html/index.html:ro" | 내 컴퓨터의 index.html을 컨테이너 안의 index.html 위치에 연결 |
| nginx:latest | nginx 이미지 사용 |

---

### 7-2. 접속 확인

<img width="664" height="374" alt="image" src="https://github.com/user-attachments/assets/48f3423a-b9b5-4874-9c42-c25b8e651b9a" />

http://localhost:8082 에 접속을 확인했다.

---

### 7-3. index.html 수정

<img width="1410" height="180" alt="image" src="https://github.com/user-attachments/assets/057804cf-4292-4dd5-a26b-5ff916a7ee50" />

index.html 파일을 수정했다.

---

### 7-4. 다시 접속 확인

<img width="686" height="422" alt="image" src="https://github.com/user-attachments/assets/eb94f955-538f-4b0a-b771-3f009f09527e" />

수정된 내용을 확인했다.

---
