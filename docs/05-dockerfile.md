## 5. Dockerfile 빌드/실행

Dockerfile을 작성해서 직접 Docker 이미지를 만들고, 컨테이너를 실행한 뒤 포트 매핑을 통해 웹페이지에 접속한다.

---

### 5-1. index.html 작성

<img width="1412" height="474" alt="image" src="https://github.com/user-attachments/assets/8b297f7f-948b-41ce-ae70-0588cf54c19c" />

nginx 웹서버에서 보여줄 HTML 파일을 만들었다.

### 5-2. Dockerfile 만들기

<img width="1402" height="184" alt="image" src="https://github.com/user-attachments/assets/ee115df5-6bd1-41cc-b801-2da9014e5cd1" />

nginx라는 웹서버 이미지를 기반으로 새 이미지를 만든다는 뜻입니다.
latest는 최신 태그를 의미합니다.

COPY index.html /usr/share/nginx/html/index.html
현재 폴더의 index.html 파일을 컨테이너 안의 nginx 기본 웹페이지 위치로 복사한다.
즉, 우리가 만든 HTML 파일을 nginx 웹서버가 보여주게 됩니다.

---

### 5-3. Docker 이미지 빌드하기

<img width="1396" height="68" alt="image" src="https://github.com/user-attachments/assets/18792086-3561-4851-b2bd-dd904f02fa0a" />

| 명령어 | 역할 |
| --- | --- |
| docker build | 이미지를 만든다 |
| -t my-nginx:v1 | 이미지 이름과 태그를 지정한다 |
| . | 현재 폴더를 빌드 컨텍스트로 사용한다 |

---

### 5-4. 컨테이너 실행하기

<img width="1414" height="104" alt="image" src="https://github.com/user-attachments/assets/6770dd41-d516-4caa-ac73-69ae175119b4" />

| 명령어 | 역할 |
| --- | --- |
| -d | 백그라운드로 실행 |
| --name web-test | 컨테이너 이름을 web-test로 지정 |
| -p 8080:80 | 내 컴퓨터의 8080 포트를 컨테이너의 80 포트와 연결 |
| my-nginx:v1 | 실행할 이미지 |

포트 매핑 구조는 "내 컴퓨터 localhost:8080 -> Docker 컨테이너 80번 포트 -> nginx 웹서버"로 된다.

---

### 5-5. 웹페이지 확인하기

<img width="856" height="404" alt="image" src="https://github.com/user-attachments/assets/57d295a2-f848-4fcc-8572-fc4d0bb86bf2" />

Windows 브라우저에서 http://localhost:8080에 접속했다.
