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

e.g. goodsList, modelStatus

### 3. 함수 명명 규칙
 1) 함수의 이름은 동사+명사로 작성한다.
 2) 두 단어 이상이 조합되면 PascalCase 표기법을 기준으로 표기한다.
   (각 단어별 첫글자가 대문자)
 3) 함축된 단어나 약어를 사용하지 않으며, 영어 단어사전에 없는 단어는 되도록 사용하지 않는다.
 
 * 추천하는 동사명
 
Create / Destroy, Open / Close, Init / Final, Play / Stop, Get / Set, Add / Remove,
Insert / Delete, Start / Stop, Suspend / Resume, Begin / End, First / Last,
Next / Previous, Increment / Decrement, Old / New, Up / Down, Min / Max, Show / Hide

e.g. GotoURL(), ViewMap(), PlayMovie(), ParseURL()


