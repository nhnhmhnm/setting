## Docker 설치/점검

이번 환경에서는 Ubuntu 내부에 Docker Engine을 직접 설치하지 않고,  
Windows의 Docker Desktop을 설치한 뒤 WSL Integration을 통해 Ubuntu 터미널에서 Docker 명령어를 사용하는 방식으로 진행했다.

처음에는 Ubuntu 내부에 Docker Engine을 직접 설치하려고 했지만,
sudo apt update 실행 중 Docker 공식 저장소 연결에서 멈추는 문제가 발생했다.

이는 Docker 저장소인 download.docker.com에 연결되지 않는 네트워크 문제로 판단했다.

따라서 WSL 환경에서 더 권장되는 방식인 Docker Desktop 방식으로 전환했다.

---

### 1. Docker 설치 

Windows에서 Docker Desktop for Windows를 설치했다.

다운로드 주소: https://www.docker.com/products/docker-desktop/

![alt text](image-5.png)

그 후 Docker Desktop에서 WSL Integration을 활성화했다.

---

### 2. Docker 버전 확인

![alt text](image-6.png)

Docker와 Docker Compose가 정상 설치된 것을 확인했다.

---

### 3. Docker 서비스 상태 확인

![alt text](image-7.png)

Docker가 실제로 동작하는지 확인하기 위해 hello-world 이미지를 실행해 Docker 서비스가 실행 중임을 확인했다.

---

### 4. 컨테이너 목록 확인

![alt text](image-8.png)

현재 실행 중인 컨테이너를 확인했다.

![alt text](image-9.png)

종료된 컨테이너까지 포함해서 확인했다.
hello-world 컨테이너는 실행 후 바로 종료되므로
docker ps에는 보이지 않고, docker ps -a에는 보일 수 있다.
