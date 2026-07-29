## 4. hello-world 실행

[Docker 설치/점검](docs/03-docker-install.md)에 이어서 hello-world 이미지를 실행한다.

---

### 4-1. Docker 서비스 상태 확인

<img width="1400" height="1194" alt="스크린샷 2026-07-29 142124" src="https://github.com/user-attachments/assets/4a0f2ba3-7a6a-4248-a81e-bd3741325d22" />

Docker가 실제로 동작하는지 확인하기 위해 hello-world 이미지를 실행해 Docker 서비스가 실행 중임을 확인했다.

---

### 4-2. 컨테이너 목록 확인

<img width="1400" height="78" alt="스크린샷 2026-07-29 142216" src="https://github.com/user-attachments/assets/b8a8a055-3b93-430b-a38b-fcb615b24160" />

현재 실행 중인 컨테이너를 확인했다.

<img width="1406" height="370" alt="스크린샷 2026-07-29 142238" src="https://github.com/user-attachments/assets/bdf76281-a211-496d-b299-42d26db3782f" />

종료된 컨테이너까지 포함해서 확인했다.
hello-world 컨테이너는 실행 후 바로 종료되므로
docker ps에는 보이지 않고, docker ps -a에는 보일 수 있다.

---
