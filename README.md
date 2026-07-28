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

```bash
$ pwd
/home/namnam
```

`pwd` 명령어를 사용하여 현재 작업 중인 디렉토리 위치를 확인했다.

---

### 3-2. 작업 디렉토리 생성 및 이동

```bash
$ mkdir codyssey
$ cd codyssey
$ pwd
/home/namnam/codyssey
```

`mkdir` 명령어로 `codyssey` 디렉토리를 생성했고, `cd` 명령어로 해당 디렉토리로 이동했다.

---

### 3-3. 디렉토리 목록 확인

```bash
$ ls
```

처음 생성한 디렉토리였기 때문에 출력되는 파일이나 폴더가 없었다.

```bash
$ ls -la
total 8
drwxr-xr-x  2 namnam namnam 4096 Jul 28 14:08 .
drwxr-x--- 10 namnam namnam 4096 Jul 28 14:08 ..
```

`ls -la` 명령어를 사용하여 숨김 항목을 포함한 상세 목록을 확인했다.

- `.` : 현재 디렉토리
- `..` : 상위 디렉토리

---

### 3-4. 하위 디렉토리 생성 및 이동

```bash
$ mkdir week1
$ ls
week1

$ cd week1
$ pwd
/home/namnam/codyssey/week1
```

`week1` 디렉토리를 생성하고 해당 디렉토리로 이동했다.

---

### 3-5. 파일 생성

```bash
$ touch hello.txt
$ ls -la
total 8
drwxr-xr-x 2 namnam namnam 4096 Jul 28 14:17 .
drwxr-xr-x 3 namnam namnam 4096 Jul 28 14:09 ..
-rw-r--r-- 1 namnam namnam    0 Jul 28 14:17 hello.txt
```

`touch` 명령어를 사용하여 빈 파일 `hello.txt`를 생성했다.

---

### 3-6. 파일 내용 작성 및 확인

```bash
$ echo "Hello World" > hello.txt
$ cat hello.txt
Hello World
```

`echo` 명령어와 리다이렉션 `>`를 사용하여 `hello.txt` 파일에 내용을 작성했다.  
`cat` 명령어로 파일 내용을 확인했다.

---

### 3-7. 파일 복사

```bash
$ cp hello.txt hello_cp.txt
$ cat hello_cp.txt
Hello World
```

`cp` 명령어를 사용하여 `hello.txt` 파일을 `hello_cp.txt`로 복사했다.

```bash
$ ls -la
total 16
drwxr-xr-x 2 namnam namnam 4096 Jul 28 14:18 .
drwxr-xr-x 3 namnam namnam 4096 Jul 28 14:09 ..
-rw-r--r-- 1 namnam namnam   12 Jul 28 14:17 hello.txt
-rw-r--r-- 1 namnam namnam   12 Jul 28 14:18 hello_cp.txt
```

복사된 파일이 정상적으로 생성된 것을 확인했다.

---

### 3-8. 파일 이름 변경

```bash
$ mv hello_cp.txt hello_copy.txt
$ ls -la
total 16
drwxr-xr-x 2 namnam namnam 4096 Jul 28 14:19 .
drwxr-xr-x 3 namnam namnam 4096 Jul 28 14:09 ..
-rw-r--r-- 1 namnam namnam   12 Jul 28 14:17 hello.txt
-rw-r--r-- 1 namnam namnam   12 Jul 28 14:18 hello_copy.txt
```

`mv` 명령어를 사용하여 `hello_cp.txt` 파일 이름을 `hello_copy.txt`로 변경했다.

---

### 3-9. 파일 삭제

```bash
$ rm hello_copy.txt
$ ls -la
total 12
drwxr-xr-x 2 namnam namnam 4096 Jul 28 14:19 .
drwxr-xr-x 3 namnam namnam 4096 Jul 28 14:09 ..
-rw-r--r-- 1 namnam namnam   12 Jul 28 14:17 hello.txt
```

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

## 5. 스크린샷

터미널 기본 조작 실행 화면이다.
<img width="1426" height="680" alt="스크린샷 2026-07-28 141237" src="https://github.com/user-attachments/assets/46625b0b-9ea5-4fe3-ae48-3ad5b12d4bc4" />
<img width="1414" height="1240" alt="스크린샷 2026-07-28 142013" src="https://github.com/user-attachments/assets/93ecacee-f94e-45aa-84ba-960fc249318a" />
