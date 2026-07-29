## 3. Docker 설치/점검

이번 환경에서는 Ubuntu 내부에 Docker Engine을 직접 설치하지 않고,  
Windows의 Docker Desktop을 설치한 뒤 WSL Integration을 통해 Ubuntu 터미널에서 Docker 명령어를 사용하는 방식으로 진행했다.

처음에는 Ubuntu 내부에 Docker Engine을 직접 설치하려고 했지만,
sudo apt update 실행 중 Docker 공식 저장소 연결에서 멈추는 문제가 발생했다.

이는 Docker 저장소인 download.docker.com에 연결되지 않는 네트워크 문제로 판단했다.

따라서 WSL 환경에서 더 권장되는 방식인 Docker Desktop 방식으로 전환했다.

---

### 3-1. Docker 설치 

Windows에서 Docker Desktop for Windows를 설치했다.

다운로드 주소: https://www.docker.com/products/docker-desktop/

<img width="1706" height="822" alt="스크린샷 2026-07-29 141934" src="https://github.com/user-attachments/assets/d66d5568-ab61-44b1-869d-b8ba4cfad3a9" />

그 후 Docker Desktop에서 WSL Integration을 활성화했다.

---

### 3-2. Docker 버전 확인

<img width="1402" height="144" alt="스크린샷 2026-07-29 142018" src="https://github.com/user-attachments/assets/6f5d0980-d687-444c-991d-f62d3cdd2f86" />

Docker와 Docker Compose가 정상 설치된 것을 확인했다.

---
