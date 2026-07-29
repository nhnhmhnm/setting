## 8. 볼륨 영속성

| 명령어 | 역할 |
| --- | --- |
| docker compose up -d | 실행 |
| docker compose ps | 상태 확인 |
| docker compose logs | 로그 확인 |
| docker compose down | 종료 및 삭제 |
| docker compose restart | 다시 시작 |

---

### 8-3. compose.yaml 파일 만들기

<img width="1404" height="334" alt="image" src="https://github.com/user-attachments/assets/f92e7c04-3507-448b-8038-d58d3af1ce1b" />

compose.yaml 파일을 생성했다.
 
---

### 8-2. Docker Compose 실행

<img width="1394" height="108" alt="image" src="https://github.com/user-attachments/assets/73cd92c7-261f-4a7c-ab08-67853bb58427" />

docker run -d --name web-bind-test -p 8082:80 -v "$(pwd)/index.html:/usr/share/nginx/html/index.html:ro" nginx:latest 대신 짧은 명령어로 실행했다.

---

### 8-3. index.html 수정 후 바로 반영 확인

<img width="726" height="438" alt="image" src="https://github.com/user-attachments/assets/43301345-0c23-42d6-b626-3266a64011e0" />

기존 8083 포트였다.

<img width="1408" height="180" alt="image" src="https://github.com/user-attachments/assets/4f324b99-6617-449f-b6ae-30ad112a1d31" />

index.html 을 수정했다.

<img width="766" height="408" alt="image" src="https://github.com/user-attachments/assets/96506080-9085-4d22-b61a-c54ef70259b3" />

수정이 반영됐다.
