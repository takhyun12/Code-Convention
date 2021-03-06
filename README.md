# Code-Convention (코드 작성 규칙)

최종수정일 : 2020/11/25

## 가. 명명 규칙 (Name Convention Rule)
### 1. 파일 명명 규칙
 1) 의미 있는 명사로 사용한다.
 2) 두 단어 이상이 조합되면 PascalCase 표기법을 기준으로 표기한다.
   (각 단어별 첫글자가 대문자)
 3) 함축된 단어나 약어를 사용하지 않으며, 영어 단어사전에 없는 단어는 되도록 사용하지 않는다.
 4) 확장자는 무조건 소문자로 저장한다.
 5) 폴더명 또한 동일한 규칙을 적용한다.

> e.g. DisplayApiController.java, DisplayService.java

### 2. 변수 명명 규칙
 1) 변수는 두 단어 이상이 조합되면 lowerCamelCase 표기법을 기준으로 표시한다.
    (기본적으로 소문자이며, 새로운 단어의 첫글자만 대문자)
 2) 명확한 의미를 포함하도록 작성한다.
 3) 함축된 단어나 약어를 사용하지 않으며, 영어 단어사전에 없는 단어는 되도록 사용하지 않는다.
 4) i, n, j, k 등의 변수명을 사용하지 않으며, index, temp 등 명확한 네임을 지정한다.
 5) 네이밍에서 "_" 언더바는 전역변수를 의미한다.
 6) 특히 bool type은 상태를 정확히 알 수 있도록 네이밍한다.

> e.g.
bool isTutorial= false, char userName[20] = {0, }, int type: int score = 0, string type: string kakaoUserId = ""

### 3. 함수 명명 규칙
 1) 함수의 이름은 동사+명사로 작성한다.
 2) 두 단어 이상이 조합되면 PascalCase 표기법을 기준으로 표기한다.
   (각 단어별 첫글자가 대문자)
 3) 함축된 단어나 약어를 사용하지 않으며, 영어 단어사전에 없는 단어는 되도록 사용하지 않는다.
 
추천하는 동사명:
Create / Destroy, Open / Close, Init / Final, Play / Stop, Get / Set, Add / Remove,
Insert / Delete, Start / Stop, Suspend / Resume, Begin / End, First / Last,
Next / Previous, Increment / Decrement, Old / New, Up / Down, Min / Max, Show / Hide

> e.g. GotoURL(), ViewMap(), PlayMovie(), ParseURL()

### 4. 상수 명명 규칙
 1) 상수는 GNU Naming Convention을 사용하며, "_" 언더바를 통해 구분한다.
 (모두 대문자로 표시)
 2) 상수는 항상 코드 상단에 모아 놓는다.
 
> e.g. DEFAULT_COUNTRY_CODE, TEST_DATA, FILE_PATH
 
 ### 5. 파라미터 명명 규칙
  1) 파라미터는 최대 4~5개를 넘기지 않으며, 반드시 필요한 것만 넘기도록 한다.
  2) 파라미터에 절대로 bool type을 넣지 않는다. 
  (bool type이 포함된 함수에는 조건문이 있으며 이해를 어렵게 함)
  3) 파라미터 또한 변수 명명 규칙을 잘 준수한다.
  4) 파라미터에 띄워쓰기를 잘 맞춰서 한다.
  
> 잘못된 예) GetMyName(param1,param2,param3);

> 올바른 예) GetMyName(param1, param2, param3);

## 나. 코드 작성 규칙 (Coding Rule)
### 1. 조건문 규칙
  1) 조건문에서 else if 조건이 5개 이상이면, switch/case문을 사용한다.
  2) 코드와 ( ) 사이 그리고 ( ) 내부에 띄워쓰기를 잘 준수한다.
  
  > 올바른 예) if( userName == "james" ) 
  * 괄호안은 띄워쓰기를 준수하였고, 코드(if)와 괄호사이는 띄워쓰기가 없도록 하였다.

  ### 2. 반복문 규칙
  1) 무한루프는 반복문 위에 주석으로 반드시 표기한다.
  2) i, n, j, k 등의 임시 변수명을 사용하지 않으며, index, temp 등 명확한 네임을 지정한다.
  3) 반복문 위에 반복 횟수와 목적을 간략하게 주석으로 기록한다.
