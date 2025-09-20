# Week04 Quiz1:

## 1. Problem:

이 프로그램은 3명의 은행 계좌 정보를 관리하는 시스템입니다.  
각 계좌는 계좌 번호, 사용자 이름, 생년월일, 잔액 정보를 포함하고 있습니다.  
3명의 계좌 정보가 배열에 저장되어 있으며, 이름, 입출금 선택, 입출금할 금액을 입력받아 작업을 수행하는 코드를 작성하세요.  
출금 시 잔액이 부족할 경우 에러 처리 한 뒤, "not enough balance" 메시지를 출력하세요.  
에러처리 후 출력하는 코드는 main에서 작성해주세요.

계좌 정보 :  
{1001, Kim, 3/7/2000, 5000}  
{1002, Lee, 5/17/2002, 8000}  
{1003, Park, 20/50/2008, 15000}  

- **BankAccount 클래스**와 **Date 클래스**를 사용하여 코드를 작성하세요.
- BankAccount(int 계좌번호, string 이름, int 월, int 일, int 년도, int 금액) 형태로 생성자를 작성하세요.
- BankAccount 클래스는 입금 함수 deposit(int), 출금 함수 withdraw(int), 잔액 조회 Check(), 모든 계좌 정보 출력하는 printAll()를 멤버 함수를 가집니다.
- Date 클래스 생성 중에 오류가 발생하면, **default 값인 1900년 1월 1일**을 대신 사용하세요.
- 순회하지 않고, 1회만 진행
- BankAccount.h, BankAccount.cpp, Date.h, Date.cpp, main.cpp 파일 만을 사용하여 코드를 작성하세요.  

### Input
사용자로부터 입금 또는 출금을 수행할 계좌의 이름과 입출금 금액을 입력받습니다.  

1. 사용자 이름  
2. 입금/출금 선택 (1: 입금, 2: 출금)  
3. 입출금할 금액  

### Output  

3명의 현재 생일 정보와 계좌 정보가 출력되게 한 다음   
입출금 작업 후의 계좌 정보를 출력합니다.  

출금 시 잔액이 부족하면 "not enough balance" 오류 메시지를 출력하고,  
다음 줄에 해당 계좌 정보를 출력하세요. (Example 2 참고)

  
### 1.1 Example 1:  

**Input:**  

```
Lee
1
3000
```

**Output:**  
```
Date object constructor for date 3/7/2000
Date object constructor for date 5/17/2002
Date object constructor for date 1/1/1900
1001, Kim, 3/7/2000, 5000
1002, Lee, 5/17/2002, 8000
1003, Park, 1/1/1900, 15000
1002, Lee, 5/17/2002, 11000
Date object destructor for date 1/1/1900
Date object destructor for date 5/17/2002
Date object destructor for date 3/7/2000
```

### 1.2 Example 2:  

**Input:**

```
Lee
2
10000
```

**Output:**
```
Date object constructor for date 3/7/2000
Date object constructor for date 5/17/2002
Date object constructor for date 1/1/1900
1001, Kim, 3/7/2000, 5000
1002, Lee, 5/17/2002, 8000
1003, Park, 1/1/1900, 15000
not enough balance
1002, Lee, 5/17/2002, 8000
Date object destructor for date 1/1/1900
Date object destructor for date 5/17/2002
Date object destructor for date 3/7/2000
```

None.

<img src="https://cdn.imweb.me/upload/S201906178853c3e170808/c5d876d707352.jpg" width=30% align=center />
