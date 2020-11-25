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

e.g. DisplayApiController.java, DisplayService.java

### 2. 변수 명명 규칙
 1) 변수는 두 단어 이상이 조합되면 lowerCamelCase 표기법을 기준으로 표시한다.
    (기본적으로 소문자이며, 새로운 단어의 첫글자만 대문자)
 2) 명확한 의미를 포함하도록 작성한다.
 3) 함축된 단어나 약어를 사용하지 않으며, 영어 단어사전에 없는 단어는 되도록 사용하지 않는다.
 4) i, n, j, k 등의 변수명을 사용하지 않으며, index, temp 등 명확한 네임을 지정한다.
 5) 네이밍에서 "_" 언더바의 사용을 하지 않는다.
 6) 특히 bool type은 상태를 정확히 알 수 있도록 네이밍한다.

e.g.
bool type: bool isTutorial= false; bool wasDisabledDueToHoverBoard = false;
char type: char userName[20] = {0, };
int type: int score = 0;
float type: float leftMoveSpeed = 5.0f;
string type: string kakaoUserId = "";
double type: double chipValue = 0;


### 3. 함수 명명 규칙
 1) 함수의 이름은 동사+명사로 작성한다.
 2) 두 단어 이상이 조합되면 PascalCase 표기법을 기준으로 표기한다.
   (각 단어별 첫글자가 대문자)
 3) 함축된 단어나 약어를 사용하지 않으며, 영어 단어사전에 없는 단어는 되도록 사용하지 않는다.
 
추천하는 동사명:
Create / Destroy, Open / Close, Init / Final, Play / Stop, Get / Set, Add / Remove,
Insert / Delete, Start / Stop, Suspend / Resume, Begin / End, First / Last,
Next / Previous, Increment / Decrement, Old / New, Up / Down, Min / Max, Show / Hide

e.g. GotoURL(), ViewMap(), PlayMovie(), ParseURL()

### 4. 상수 명명 규칙
 1) 상수는 GNU Naming Convention을 사용하며, "_" 언더바를 통해 구분한다.
 (모두 대문자로 표시)
 2) 상수는 항상 코드 상단에 모아 놓는다.
 
 e.g. DEFAULT_COUNTRY_CODE, TEST_DATA, FILE_PATH
 
 ### 5. 파라미터 명명 규칙
  1) 파라미터는 최대 4~5개를 넘기지 않으며, 반드시 필요한 것만 넘기도록 한다.
  2) 파라미터에 절대로 bool type을 넣지 않는다. 
  (bool type이 들어가게 되면, 함수에 조건문이 반드시 있다는것을 의미)
  3) 파라미터 또한 변수 명명 규칙을 잘 준수한다.
  4) 파라미터에 띄워쓰기를 잘 맞춰서 한다.
  
  
잘못된 예)
GetMyName(param1,param2,param3);

올바른 예)
GetMyName(param1, param2, param3);

## 나. 코드 작성 규칙 (Coding Rule)
### 1. 파일 명명 규칙
  
