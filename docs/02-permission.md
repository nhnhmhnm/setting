## 2. 권한 변경

| 숫자 | 문자 | 의미 |
|---|---|---|
| 4 | `r`	read | 읽기 |
| 2 | `w`	write | 쓰기 |
| 1 | `x`	execute | 실행 |
| 0 | `-` |	권한 없음 |

---

### 2-1. 파일 권한 확인

<img width="1412" height="118" alt="image" src="https://github.com/user-attachments/assets/c0c69c90-c3f1-4dbc-97be-f1dffbdd84ed" />

`ls -l` 명령어로 파일의 권한을 확인했다.

---

### 2-2. 권한 변경

<img width="1418" height="160" alt="image" src="https://github.com/user-attachments/assets/5b19d241-8791-4391-b460-238cb9de7276" />

소유자 권한에서 쓰기 권한을 제거했다.

<img width="1410" height="80" alt="image" src="https://github.com/user-attachments/assets/5f4d74fd-4e1c-4f10-b26d-8d476bb7629e" />

쓰기 권한이 없어서 파일 수정이 거부되었다.

<img width="1418" height="196" alt="image" src="https://github.com/user-attachments/assets/81e075f6-aff0-415c-bc73-ede8406aa6f8" />

쓰기 권한을 다시 부여해 파일을 수정했다.

<img width="1420" height="34" alt="image" src="https://github.com/user-attachments/assets/1a5aae3b-339f-4a04-8e6f-202169c6642f" />

숫자로도 권한을 부여할 수 있다.  
앞에서부터 소유자, 그룹, 기타 사용자에게 읽기(4) + 쓰기(2) + 실행(1)의 권한을 부여한다.  

---
