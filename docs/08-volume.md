## 8. 볼륨 영속성

컨테이너 안에만 파일을 만들면: 컨테이너를 삭제하면 파일이 삭제된다.  
볼륨에 파일을 만들면: 컨테이너를 삭제하면 파일은 볼륨에 남아있고 다른 컨테이너에서 다시 사용 가능하다.

---

### 8-3. 볼륨 만들기

<img width="1458" height="252" alt="image" src="https://github.com/user-attachments/assets/83d6817f-6d18-4450-a591-85ca6c63abab" />

Docker가 관리하는 저장공간을 하나 만들었다.

---

### 8-2. 볼륨에 파일 저장하기

<img width="1396" height="72" alt="image" src="https://github.com/user-attachments/assets/c7901061-30d4-4660-b5d2-0f4d31d7c57f" />


alpine이라는 아주 가벼운 리눅스 컨테이너를 사용했다.

---

### 8-3. 새 컨테이너에서 데이터 확인하기

<img width="1400" height="104" alt="image" src="https://github.com/user-attachments/assets/5fabbf3a-b8be-4643-8bab-648f44dd9173" />

새로운 컨테이너로 같은 볼륨을 연 결과 Hello Docker Volume 가 나왔다.

---

### 8-4. 볼륨 상세 정보 확인

<img width="1416" height="440" alt="image" src="https://github.com/user-attachments/assets/849a0d80-2fe6-4615-8e46-91b25b52e103" />

---

### 8-5. 볼륨 삭제하기

<img width="1424" height="66" alt="image" src="https://github.com/user-attachments/assets/dd81ac3b-f81b-4403-af5e-522da76e934b" />

---
