## 1. 터미널 기본 조작

| 명령어 | 역할 |
|---|---|
| `pwd` | 현재 작업 디렉토리 확인 |
| `mkdir` | 디렉토리 생성 |
| `cd` | 디렉토리 이동 |
| `ls` | 파일 및 디렉토리 목록 확인 |
| `ls -la` | 숨김 항목과 권한 정보를 포함하여 목록 확인 |
| `touch` | 빈 파일 생성 |
| `echo` | 문자열 출력 또는 파일에 내용 작성 |
| `cat` | 파일 내용 출력 |
| `cp` | 파일 복사 |
| `mv` | 파일 이동 또는 이름 변경 |
| `rm` | 파일 삭제 |

---

### 1-1. 현재 위치 확인

<img width="1418" height="78" alt="스크린샷 2026-07-28 172515" src="https://github.com/user-attachments/assets/97542814-8cff-4985-8d2d-541cc5a661b6" />

`pwd` 명령어를 사용하여 현재 작업 중인 디렉토리 위치를 확인했다.

---

### 1-2. 디렉토리 관리

<img width="1410" height="154" alt="스크린샷 2026-07-28 172627" src="https://github.com/user-attachments/assets/0289a7ea-4969-475c-a168-c2aaab68e4f0" />

`mkdir` 명령어로 `codyssey` 디렉토리를 생성했고, `cd` 명령어로 해당 디렉토리로 이동했다.

<img width="1420" height="236" alt="image" src="https://github.com/user-attachments/assets/82c0a168-26c8-4c44-8e51-1425107b4197" />

`week1` 디렉토리를 생성하고 해당 디렉토리로 이동했다.

<img width="1424" height="122" alt="image" src="https://github.com/user-attachments/assets/1df72cb8-0534-473c-9416-32b1435a945b" />

<img width="1408" height="114" alt="image" src="https://github.com/user-attachments/assets/5dfce05a-aa4f-4866-a588-60493cd8429d" />

`cd` 명령어로 디렉토리를 이동했다.
- `~` : 홈 디렉토리
- `.` : 현재 디렉토리
- `..` : 상위 디렉토리

---

<img width="1418" height="36" alt="스크린샷 2026-07-28 172854" src="https://github.com/user-attachments/assets/8a866237-98f7-4396-bf3f-213d7256f622" />

처음 생성한 디렉토리였기 때문에 출력되는 파일이나 폴더가 없었다.

<img width="1400" height="156" alt="스크린샷 2026-07-28 172929" src="https://github.com/user-attachments/assets/5d5b4c77-32b5-484e-b28c-82735f8b3fde" />

`ls -la` 명령어를 사용하여 숨김 항목을 포함한 상세 목록을 확인했다.

---

### 1-3. 파일 관리

<img width="1178" height="198" alt="image" src="https://github.com/user-attachments/assets/44392b14-4f61-4e56-b3b9-5adcef4f95c1" />

`touch` 명령어를 사용하여 빈 파일 `hello.txt`를 생성했다.

---

<img width="1176" height="102" alt="image" src="https://github.com/user-attachments/assets/349ba5b2-44f0-4f74-980c-5696a9e9c4f7" />

`echo` 명령어와 리다이렉션 `>`를 사용하여 `hello.txt` 파일에 내용을 작성했다.  
`cat` 명령어로 파일 내용을 확인했다.


<img width="1174" height="96" alt="image" src="https://github.com/user-attachments/assets/f3c9abd7-6fc8-4ad0-96af-dfeeb20f721c" />

`cp` 명령어를 사용하여 `hello.txt` 파일을 `hello_cp.txt`로 복사했다.

<img width="1162" height="196" alt="image" src="https://github.com/user-attachments/assets/afb7d359-744b-46cc-b234-9c595f1903cc" />

복사된 파일이 정상적으로 생성된 것을 확인했다.


<img width="1170" height="232" alt="image" src="https://github.com/user-attachments/assets/717ea645-dcc9-48f9-be43-796e1e6c195a" />

`mv` 명령어를 사용하여 `hello_cp.txt` 파일 이름을 `hello_copy.txt`로 변경했다.


<img width="1170" height="196" alt="스크린샷 2026-07-28 173555" src="https://github.com/user-attachments/assets/203a38aa-0e10-40bd-af30-60f09e7d35ac" />

`rm` 명령어를 사용하여 `hello_copy.txt` 파일을 삭제했다.  
최종적으로 `hello.txt` 파일만 남아 있는 것을 확인했다.

---

### 1-4. 패키지 관리

<img width="1422" height="76" alt="image" src="https://github.com/user-attachments/assets/a8501fc6-94ab-43a3-b471-d7c44697bc2c" />

`apt update` 명령어를 사용하여 Ubuntu 패키지 목록을 최신 상태로 업데이트했다.

<img width="1406" height="82" alt="image" src="https://github.com/user-attachments/assets/61e5ce4d-0e81-4368-be52-546f56ab225d" />

`apt install` 명령어를 사용하여 개발 도구를 설치했다.
설치한 도구는 다음과 같다.

| 도구 | 역할 |
|---|---|
| git | 소스 코드 버전 관리 |
| curl | URL 요청 및 데이터 다운로드 |
| wget | 파일 다운로드 |
| vim | 터미널 텍스트 편집기 |
| tree | 디렉토리 구조 출력 |
| build-essential | 컴파일 및 빌드 도구 모음 |

<img width="1422" height="84" alt="image" src="https://github.com/user-attachments/assets/0aa5367e-6ac9-482a-b8e8-2d7adced9986" />

`--version` 명령어를 사용하여 버전을 확인할 수 있다.

---