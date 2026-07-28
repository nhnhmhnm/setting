# setting

# 개발 워크스테이션 구축 미션

## 1. 실행 환경

- OS: Ubuntu 22.04.3 LTS
- Shell: bash
- 작업 디렉토리: `/home/namnam/codyssey/week1`

---

## 2. 수행 체크리스트

- [x] 현재 디렉토리 확인
- [x] 작업 디렉토리 생성
- [x] 디렉토리 이동
- [x] 파일 생성
- [x] 파일 내용 작성
- [x] 파일 내용 확인
- [x] 파일 복사
- [x] 파일 이름 변경
- [x] 파일 삭제
- [x] 숨김 파일 포함 목록 확인

---

## 3. 터미널 기본 조작 로그

### 3-1. 현재 위치 확인

<img width="1418" height="78" alt="스크린샷 2026-07-28 172515" src="https://github.com/user-attachments/assets/97542814-8cff-4985-8d2d-541cc5a661b6" />

`pwd` 명령어를 사용하여 현재 작업 중인 디렉토리 위치를 확인했다.

---

### 3-2. 작업 디렉토리 생성 및 이동

<img width="1410" height="154" alt="스크린샷 2026-07-28 172627" src="https://github.com/user-attachments/assets/0289a7ea-4969-475c-a168-c2aaab68e4f0" />

`mkdir` 명령어로 `codyssey` 디렉토리를 생성했고, `cd` 명령어로 해당 디렉토리로 이동했다.

---

### 3-3. 디렉토리 목록 확인

<img width="1418" height="36" alt="스크린샷 2026-07-28 172854" src="https://github.com/user-attachments/assets/8a866237-98f7-4396-bf3f-213d7256f622" />

처음 생성한 디렉토리였기 때문에 출력되는 파일이나 폴더가 없었다.

<img width="1400" height="156" alt="스크린샷 2026-07-28 172929" src="https://github.com/user-attachments/assets/5d5b4c77-32b5-484e-b28c-82735f8b3fde" />

`ls -la` 명령어를 사용하여 숨김 항목을 포함한 상세 목록을 확인했다.

- `.` : 현재 디렉토리
- `..` : 상위 디렉토리

---

### 3-4. 하위 디렉토리 생성 및 이동

<img width="1420" height="236" alt="image" src="https://github.com/user-attachments/assets/82c0a168-26c8-4c44-8e51-1425107b4197" />

`week1` 디렉토리를 생성하고 해당 디렉토리로 이동했다.

---

### 3-5. 파일 생성

<img width="1178" height="198" alt="image" src="https://github.com/user-attachments/assets/44392b14-4f61-4e56-b3b9-5adcef4f95c1" />

`touch` 명령어를 사용하여 빈 파일 `hello.txt`를 생성했다.

---

### 3-6. 파일 내용 작성 및 확인

<img width="1176" height="102" alt="image" src="https://github.com/user-attachments/assets/349ba5b2-44f0-4f74-980c-5696a9e9c4f7" />

`echo` 명령어와 리다이렉션 `>`를 사용하여 `hello.txt` 파일에 내용을 작성했다.  
`cat` 명령어로 파일 내용을 확인했다.

---

### 3-7. 파일 복사

<img width="1174" height="96" alt="image" src="https://github.com/user-attachments/assets/f3c9abd7-6fc8-4ad0-96af-dfeeb20f721c" />

`cp` 명령어를 사용하여 `hello.txt` 파일을 `hello_cp.txt`로 복사했다.

<img width="1162" height="196" alt="image" src="https://github.com/user-attachments/assets/afb7d359-744b-46cc-b234-9c595f1903cc" />

복사된 파일이 정상적으로 생성된 것을 확인했다.

---

### 3-8. 파일 이름 변경

<img width="1170" height="232" alt="image" src="https://github.com/user-attachments/assets/717ea645-dcc9-48f9-be43-796e1e6c195a" />

`mv` 명령어를 사용하여 `hello_cp.txt` 파일 이름을 `hello_copy.txt`로 변경했다.

---

### 3-9. 파일 삭제

<img width="1170" height="196" alt="스크린샷 2026-07-28 173555" src="https://github.com/user-attachments/assets/203a38aa-0e10-40bd-af30-60f09e7d35ac" />

`rm` 명령어를 사용하여 `hello_copy.txt` 파일을 삭제했다.  
최종적으로 `hello.txt` 파일만 남아 있는 것을 확인했다.

---

## 4. 이번 단계에서 사용한 명령어 정리

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

## 5. 
