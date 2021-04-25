# WCAG 2.1
WCAG 는 웹 콘텐츠의 접근성을 향상시키기 위한 권고안입니다. 이 지침은 전맹, 저시력, 청각 장애, 청각 손실, 운동 장애, 언어 장애 등의 문제가 있는 사람 뿐 아니라, 학습 장애, 인지 능력 장애가 있는 사람까지 컨텐츠에 쉽게 접근할 수 있게 됩니다. 

WCAG의 각 원칙을 지키기 위해서는 여러가지 지침을 지켜야 하고, 해당 지침들은 특정 적합 기준을 이용해서 테스트 가능하게 만들어져 있습니다. 

## WCAG 2.0 과의 차이
WCAG 2.1 은 WCAG 2.0의 보완 버전입니다. 때문에 WCAG 2.0을 더 이상 사용하지 못하거나 하지는 않습니다. 하지만 W3C 는 WCAG의 최신 버전을 사용할 것을 권고하고 있습니다.

## 가이드 종류
WCAG 2.1은 광범위한 사용자(웹 디자이너, 개발자, 정책 입안자) 를 지원하기 위해 전반적인 원칙을 정하고, 이를 지키기 위한 지침을 정의합니다. 또한 이런 지침을 지키고 있는지 아닌지 명학하게 하기 위하여, 적합 기준 등을 제공해 이를 테스트할 수 있게 만들어줍니다. 
### 원칙
원칙은 웹 접근성의 기초를 다루기 위해 정해졌습니다. 총 네 가지의 원칙이 있고, 그 원칙은 인지 가능, 조작 가능, 이해 가능, 견고함이 있습니다. 
### 지침
지침은 위의 4가지 원칙을 지키기 위한 13개의 지침이 있습니다. 이 지침들은 기본적으로 접근성 좋은 컨텐츠를 사용자에게 제공하기 위한 목표가 됩니다. 
### 적합 기준
해당 13개의 지침을 맞추고 있는지 개발자는 확인을 할 필요가 있습니다. 이를 위해 WCAG 는 해당 지침을 맞추는 것을 확인하기 위한 적합 기준을 제공합니다. 또한 이런 지침을 어떤 수준으로 맞추고 있는지도 3단계에 나눠서 제공합니다.

#### 목차
1. [인지 가능](#1-인지-가능)
2. [조작 가능](#2-조작-가능)
3. [이해 가능](#3-이해-가능)
4. [견고함](#4-견고함)

## 3. 이해 가능

정보와 UI 조작은 이해할 수 있어야 합니다.

### 지침 3.1 가독성

Level A

텍스트 콘텐츠를 읽을 수 있고 이해할 수 있게 만듭니다.

#### 적합 기준 Criterion 3.1.1 페이지의 언어

[How to Meet Language of Page](https://www.w3.org/WAI/WCAG21/quickref/?showtechniques=311#language-of-page)각 웹 페이지의 기본 언어를 프로그래밍 방식으로 확인할 수 있습니다.

이 적합 기준의 목적은 사용자 에이전트가 텍스트 및 기타 언어 콘텐츠를 올바르게 제시하기 위해 필요한 정보를 콘텐츠 개발자가 웹 페이지에 제공할 수 있도록 하는 것입니다. 텍스트를 합성 음성으로 변환하는 스크린 리더 기술을 사용하는 사람에게 유용합니다.

**예시**

|![애플 공식 홈페이지 언어](images/apple_3.1.1.png)|
|:--:|
|애플 공식 홈페이지 요소 검사 화면|

`lang="ko-KR"`을 통해 HTML에서 웹 페이지의 기본 언어를 설저애주었음을 볼 수 있습니다.

#### 적합 기준 Criterion 3.1.2 부분의 언어

Level AA

[How to Meet Language of Parts](https://www.w3.org/WAI/WCAG21/quickref/#language-of-parts)고유명사, 기술 용어, 알 수 없는 단어의 단어, 주변 텍스트의 언어에 포함된 단어나 구절을 제외하고, 콘텐츠에 포함된 각 구절의 언어를 프로그래밍 방식으로 확인 할 수 있습니다.

이 성공 기준의 목적은 사용자 에이전트가 여러 언어로 쓰여진 콘텐츠를 올바르게 제시할 수 있도록 하는 것입니다. 문자와 알파벳 인식, 단어나 어구를 해독하고 이해하는 것이 어려운 사람들을 위해 필요합니다.

**예시**


|![네이버 영어 사전](images/naver_3.1.2.png)|
|:--:|
|네이버 영어 사전|

한글로 선언된 문서 안에 영어 문자가 쓰인 부분은 `lang` 속성이 영어로 설정됨을 볼 수 있습니다.

#### 적합 기준 3.1.3 특이한 단어

Level AAA

[How to Meet Unusual Words](https://www.w3.org/WAI/WCAG21/quickref/#unusual-words)관용구와 전문 용어(jargon) 등 보편적이지 않거나 제한된 방식으로 사용된 단어나 구절의 구체적인 정의를 확인하기 위한 메커니즘을 이용할 수 있습니다.

장애로 인해 관용어 또는 특정한 단어의 뜻을 이해하는 것이 어려울 수 있습니다. 이러한 사람들을 위해 꼭 필요한 적합 기준입니다.

**예시**

|![디스커버리 기사](images/discovery_3.1.3.png)|
|:--:|
|Environmentalists Who Changed (and Continue to Change) the World|

`WE ACT for Environmental Justice`단체에 대한 설명을 덧붙이고 있습니다.

#### 적합 기준 3.1.4 약어

Level AAA

[How to Meet Abbreviations](https://www.w3.org/WAI/WCAG21/quickref/#abbreviations)약어의 확장된 형태나 의미를 확인하는 메커니즘을 이용할 수 있습니다.(Level AAA)

이 적합 기준의 목적은 사용자가 약어의 원래 뜻을 알 수 있도록 하는 것입니다. 난독증이 있는 사람들에게 필요합니다.

**예시**

|![디스커버리 기사](images/discovery_3.1.4.png)|
|:--:|
|First Dog in the US Tests Positive for Coronavirus|

`MESSI`라는 약어에 대한 설명을 덧붙이고 있습니다.

#### 적합 기준 3.1.5 읽기 수준

Level AAA

[How to Meet Reading Level](https://www.w3.org/WAI/WCAG21/quickref/#reading-level)고유명사와 제목을 제외하고 텍스트를 이해하는 데 중등 교육(중학교) 수준 이상의 독해력이 필요한 경우 이를 보완하는 콘텐츠 또는 그러한 독해력이 필요하지 않은 버전을 이용할 수 있습니다.

일반적인 지식이나 구체적인 정보를 얻기 위해 쓰는 말(텍스트나 점자에 의한 기사, 설명서, 신문 등)을 이해하고 해석하는 것이 어려운 사람들이 있습니다. 이 분들을 위해 어려운문장이나 복잡한 문장의 추가내용을 이용할 수 있도록 해야합니다.

**예시**

|![네이처 기사](./images/nature_3.1.5.png)|
|---|
|네이처 기사 일부 발췌|

기술적인 기사에 `Abstract`를 달아줌으로써 이해를 돕습니다.

#### 적합 기준 3.1.6 발음

Level AAA

[How to Meet Pronunciation](https://www.w3.org/WAI/WCAG21/quickref/#pronunciation)발음을 모르면 문맥에서 단어의 의미가 모호한 경우 단어의 구체적인 발음을 확인하는 메커니즘을 이용할 수 있습니다.

이 적합 기준의 목적은 눈이 먼 사람, 시력이 낮은 사람,독해력이 없는 사람이 발음에 따라 의미가 다를 때 내용을 이해할 수 있도록 하는 것입니다.

**예시**

|![다음 일본어 사전](images/daum_dict_3.1.6.png)|
|:--:|
|다음 일본어 사전 검색 결과|

오후를 나타내는 한자를 히라가나로도 표시하여 발음을 쉽게 파악할 수 있게 합니다.

### 지침 3.2 예측 가능성

웹 페이지가 예측 가능한 방식으로 나타나고 작동되게 합니다.

#### 적합 기준 3.2.1 포커스 시

Level A

[How to Meet On Focus](https://www.w3.org/WAI/WCAG21/quickref/#on-focus)컴포넌트가 포커스를 받으면 컨텍스트를 변경하지 않습니다.

이 적합 기준의 목적은 방문자가 문서를 네비게이트할 때 기능이 예측 가능함을 확인하는 것입니다. 이 적합 기준은 시각 장애, 인지 장애, 운동 장애를 가진 사람들을 지원하여 예상치 못한 상황 변화가 일어날 가능성을 줄입니다.

**예시**

|![구글 로그인 화면](images/google_3.2.1.png)|
|:--:|
|구글 로그인 화면|

계정 만들기에 포커스가 있을 때, 계정을 만드는 창을 따로 띄우지 않고 클릭이나 키보드 동작을 했을 때만 띄웁니다.

#### 적합 기준 3.2.2 입력 시

Level A

[How to Meet On Input](https://www.w3.org/WAI/WCAG21/quickref/#on-focus)사용자 인터페이스 컴포넌트의 설정을 변경해도 사용자가 해당 컴포넌트를 사용하기 전에 설정 변경에 관한 안내를 받지 않았다면 컨텍스트가 자동으로 변경되지 않는다.

이 적합 기준의 목적은 데이터 입력 또는 폼 제어 선택을 통해 예측 가능한 효과를 얻을 수 있도록 하는 것입니다. 인터랙티브 컨텐츠를 보다 예측 가능하게 함으로써 시각 장애 또는 인지 장애를 가진 사용자에게 혼란을 주지 않습니다.

**예제**

|![구글 지원서 화면](images/google_3.2.2.png)|
|:--:|
|구글 지원서 화면|

법적 성명을 입력하고 별명을 입력할 때, 법적 성명에 적은 내용이 변하지 않습니다.

#### 적합 기준 3.2.3 일관된 탐색

Level AA

[How to Meet Consistent Navigation](https://www.w3.org/WAI/WCAG21/quickref/#consistent-navigation)일련의 웹 페이지 내에서 여러 웹 페이지에 반복되는 탐색 메커니즘은 사용자가 변경을 개시하지 않는 한 반복될 때마다 동일한 상대 순서로 발생합니다.

이 적합 기준의 목적은 일련의 웹 페이지 내에서 반복적으로 콘텐츠를 조작하고 특정 정보 또는 기능을 여러 번 검색해야 하는 사용자에게 일관된 프레젠테이션과 레이아웃 사용을 장려하는 것입니다. 이 기준을 준수하면 사이트의 각 페이지에서 컴포넌트가 같은 순서로 반복되도록 함으로써 사용자는 각 페이지의 어디에 무엇이 있는지를 예측할 수 있게 됩니다.

**예제**

|![우체국 홈페이지](images/post_office_3.2.3.png)|
|:--:|
|우체국 홈페이지 보이스 오버 사용 화면|

우체국에서 어느 콘텐츠에 들어가 있던, `주 메뉴 바로가기`, `본문 내용 바로가기`, `하단 내용 바로가기`로 들어가고자 하는 내용에 빠르게 들어갈 수 있습니다.

#### 적합 기준 3.2.4 일관된 식별

Level AA

[How to Meet Consistent Identification](https://www.w3.org/WAI/WCAG21/quickref/#consistent-identification)일련의 웹 페이지 내에서 기능이 동일한 컴포넌트는 동일하게 식별합니다.

이 적합 기준의 목적은 일련의 웹 페이지에 반복적으로 표시되는 기능 컴포넌트를 일관되게 식별하는 것입니다. 이러한 식별은 사이트의 한 페이지에서 기능을 학습하면 사용자는 별도의 추가 교육 없이 다른 페이지에서 기능을 찾아볼 수 있습니다.

**예제**


|![크롬 다운로드](images/google_3.2.4.png)|
|:--:|
|크롬 다운로드 문서|

|![김데레사님의 블로그](images/deresa_3.2.4.png)|
|:--:|
|김데레사님 블로그 포스트 일부 발췌|

링크를 통해 넘어가는 곳에 같은 아이콘이 사용된 것을 볼 수 있습니다.

#### 적합 기준 3.2.5 요청 시 변경

Level AAA

[How to Meet Change on Request](https://www.w3.org/WAI/WCAG21/quickref/#change-on-request)컨텍스트의 변경이 사용자 요청에 의해서만 일어나거나 그러한 변화를 중지할 수 있는 메커니즘을 이용할 수 있다.

이 적합 기준의 목적은 사용자가 콘텍스트의 변경을 완전히 제어할 수 있는 Web 컨텐츠의 설계를 촉진하는 것입니다. 콘텍스트의 변경을 검출할 수 없는 경우, 또는 콘텍스트의 변경을 눈치채지 못한 경우에 주는 혼란을 방지할 수 있습니다.

**예시**

|![네이버 프로필 수정](images/naver_3.2.5.png)|
|:--:|
|네이버 프로필 수정 화면|

프로필 수정에서 별명 내용을 변경하더라도 적용 버튼을 누르기 전까진 적용하지 않습니다.

### 지침 3.3 입력 지원

사용자가 실수를 피하고 바로잡을 수 있게 돕습니다.

#### 적합 기준 3.3.1 오류 확인

Level A

[How to Meet Error Identification](https://www.w3.org/WAI/WCAG21/quickref/#error-identification)입력 오류가 자동으로 감지되면 오류가 있는 항목을 식별하고 사용자에게 오류를 텍스트로 설명합니다.

이 적합 기준의 목적은 오류가 발생했다는 것을 사용자가 인식하고 무엇이 잘못되었는지를 판단할 수 있도록 하는 것입니다. 예를 들어 이메일을 적는 란에 이메일 양식이 올바르지 않음을 상기시켜 줄 수 있습니다.

**예제**

|![네이버 이메일 수정 창](images/naver_3.3.1.png)|
|:--:|
|네이버 이메일 수정 창|

이메일 형식에 맞지 않은 정보를 입력하면 이메일 형식이 올바르지 않음을 알려줍니다.

#### 적합 기준 3.3.2 레이블 또는 지침

Level A

[How to Meet Labels or Instructions](https://www.w3.org/WAI/WCAG21/quickref/#labels-or-instructions)사용자 입력이 필요한 콘텐츠에는 레이블이나 지침이 제공됩니다.

이 적합 기준의 목적은 콘텐츠 작성자에게 컨트롤을 식별하는 절차 또는 라벨을 제시하여 사용자가 원하는 입력 데이터를 파악할 수 있도록 하는 것입니다. 명확한 식별이나 지침은 모든 사용자들에게 올바느 정보를 입력할 수 있도록 돕습니다.

|![구글 채용 창](images/google_3.3.2.png)|
|:--:|
|구글 채용 경력 날짜 입력 칸|

날짜 입력에 대해서 월과 연도에 대한 힌트를 주고 있습니다. 추가로 연도에는 입력 서식에 대한 힌트도 적혀있습니다.

#### 적합 기준 3.3.3 오류 추천 항목

Level AA

[How to Meet Error Suggestion](https://www.w3.org/WAI/WCAG21/quickref/#labels-or-instructions)입력 오류가 자동으로 감지되고 이를 정정하기 위한 추천 항목이 있다면 그 추천 항목이 콘텐츠의 보안이나 목적을 위태롭게 하지 않는 한 이를 사용자에게 제공합니다.

이 성공 기준의 목적은 가능하면 입력 오류를 수정하기 위한 적절한 제안을 사용자에게 제공하는 것입니다. 입력 오류 수정 방법에 대한 정보를 제공하면 학습 장애를 가진 사용자가 양식에 맞게 입력할 수 있습니다.

**예시**

|![데한민국 구글 검색 결과](images/google_3.3.3.png)|
|:--:|
|데한민국 구글 검색 결과|

검색어를 '데한민국'이라고 하였을 때 '대한민국'으로 수정된 결과가 나옵니다.

#### 적합 기준 3.3.4 오류 방지(법률, 금융, 데이터)

Level AA

**예시**

[How to Meet Error Prevention (Legal,Financial, Data)](https://www.w3.org/WAI/WCAG21/quickref/#error-prevention-legal-financial-data)사용자에 대한 법적 책임이나 금융 거래가 발생하는 웹 사이트가 데이터 스토리지 시스템에서 사용자가 제어할 수 있는 데이터를 수정 또는 삭제하거나 사용자 테스트 응답을 제출하는 경우, 다음 중 하나 이상을 만족합니다.

- 복원 가능(Reversible): 제출 내역을 복원할 수 있습니다.
- 점검(Checked): 사용자가 입력한 데이터에 입력 오류가 있는지 점검하고 오류를 수정할 수 있는 기회를 사용자에게 제공합니다.
- 확인(Confirmed): 제출을 완료하기 전에 정보를 검토, 확인, 수정하는 메커니즘을 이용할 수 있습니다.

이 성공기준의 목적은 장애를 가진 사용자가 되돌릴 수 없는 액션을 실행할 때 실수로 인한 중대한 결과를 회피할 수 있도록 하는 것입니다.

**예시**

|![무신사 구매 확정 창](images/musinsa_3.3.4.png)|
|:--:|
|무신사 구매 확정 창|

무신사에서 상품을 결제하면 배송전에 주소지를 수정할 수 있으며, 구매 확정을 하려고 하면 정보가 맞는지 검토할 수 있는 팝업창이 나타납니다.

#### 적합 기준 3.3.5 도움말

Level AAA

[How to Meet Error Prevention (All)](https://www.w3.org/WAI/WCAG21/quickref/#error-prevention-all)사용자가 정보를 제출해야 하는 웹 페이지의 경우 다음 중 하나 이상을 만족합니다.

- 복원 가능(Reversible): 제출 내역을 복원할 수 있습니다.
- 점검(Checked): 사용자가 입력한 데이터에 입력 오류가 있는지 점검하고 오류를 수정할 수 있는 기회를 사용자에게 제공합니다.
- 확인(Confirmed): 제출을 완료하기 전에 정보를 검토, 확인, 수정하는 메커니즘 이용할 수 있습니다.

사용자가 실수를 방지하도록 하는 기준입니다. 텍스트 입력 지원은 텍스트 입력이 필요한 폼이나 다른 곳에서 텍스트를 쓰기 어려운 경우에 글쓰기 장애나 지적 장애가 있는 사람들을 지원합니다.

**예시**

|![11번가 회원가입 화면](images/11st_3.3.6.png)|
|:--:|
|11번가 회원가입 화면|

이력서를 제출하고 난 뒤, 내용을 수정할 수 있는 메커니즘을 제공합니다.

## 4. 견고함

### 지침 4.1 호환성

보조 기술을 포함해, 현재와 미래의 사용자 에이전트와의 호환성을 극대화한다.

#### 적합 기준 4.1.1 파싱

Level A

[How to Meet Parsing](https://www.w3.org/WAI/WCAG21/quickref/#parsing)마크업 언어를 이용해 구현한 요소에는 완전한 시작/종료 태그가 있고, 요소의 중첩 구조는 표준에 따라 만들어지며, 요소에 중복된 속성은 포함되지 않습니다. 또한 표준에서 허용한 경우를 제외하고, 모든 ID의 값은 고유합니다.

이 적합 기준의 목적은 지원 기술을 포함한 사용자 에이전트가 콘텐츠를 정확하게 해석 및 해석할 수 있도록 하는 것입니다.

참고

닫는 괄호처럼 태그 형성에 필수적인 문자가 빠진 시작/종료 태그나 일치하지 않는 속성 값 물음표는 완전하지 않습니다.

**예시**

|![w3 HTML 유효성 검사 이미지](images/w3_4.1.1.png)|
|:--:|
|W3C HTML 유효성 검사 결과창|

마크업 언어에서 어떠한 에러도 발생하지 않은 것을 볼 수 있습니다.

#### 적합 기준 4.1.2 이름, 역할, 값

Level A

[How to Meet Name, Role, Value](https://www.w3.org/WAI/WCAG21/quickref/#name-role-value)모든 사용자 인터페이스 컴포넌트(다음 항목을 포함하되 여기에 국한되지 않음: 스크립트로 생성한 폼 요소, 링크, 컴포넌트)에 대해, 이름(name)과 역할(role)을 프로그래밍 방식으로 확인할 수 있고, 사용자가 설정할 수 있는 상태(states)와 프로퍼티(properties), 값(values)을 프로그래밍 방식으로 설정할 수 있으며, 이러한 항목들이 변경되었을 때는 보조 기술을 포함한 사용자 에이전트에 알림이 제공됩니다.

이 적합 기준의 목적은 Assistive Technologies(AT; 보조 기술)가 콘텐츠 내 사용자 인터페이스 제어 상태에 대한 정보를 수집하고 활성화(또는 설정)하여 최신 상태를 유지할 수 있도록 하는 것입니다.

**예시**

|![스코프 요소 검사 이미지](images/scope_4.1.2.png)|
|:--:|
|스코프 사이트의 요소 검사 이미지 화면|

`aria`속성을 이용하여 보조기기로도 웹 페이지의 각 요소의 역할이나 내용을 파악할 수 있습니다.

#### 적합 기준 4.1.3 상태 메시지

Level AA

상태 메시지 이해하기[How to Meet Status Messages](https://www.w3.org/WAI/WCAG21/quickref/#status-messages)마크업 언어로 구현된 콘텐츠에서 상태 메시지는 역할이나 속성을 통해 프로그래밍 방식으로 확인할 수 있으므로 포커스를 받지 않고 보조 기술로 사용자에게 제공할 수 있습니다.

이 적합 기준의 목적은 초점이 맞춰지지 않은 콘텐츠의 중요한 변경을 사용자들에게 인식시키고 불필요하게 작업을 중단하지 않도록 하는 것입니다. 상태 메시지에 적절한 역할 또는 속성이 연결되면  새로운 콘텐츠가 스크린 리더에 의해 재생됩니다.

**예시**

|![보이스 오버로 구글 창 열기](images/google_4.1.3.png)|
|:--:|
|보이스 오버로 구글 창 열기|

사파리에서 새탭을 열고 구글을 검색하고 들어오면 새탭이 구글로 전환되고 텍스트 상자에 메시지를 입력할 수 있다는 것을 사용자에게 알려줍니다.

<details>
<summary>참고자료</summary>

<a href="https://nuli.navercorp.com/community/article/1132999%22%3EWCAG" >2.1 한글 번역</a>
<br>
<a href="https://www.w3.org/TR/WCAG21/#background-on-wcag-2%22%3EW3C"> WCAG 2.1</a>
<br>
<a href="https://www.11st.co.kr">11번가</a>
<br>
<a href="https://www.apple.com">애플</a>
<br>
<a href="https://dic.daum.net">다음 어학사전</a>
<br>
<a href="https://seulbinim.github.io/WSA/table.html#scope-id-headers-속성">테이블 관련 요소</a>
<br>
<a href="https://www.discovery.com/nature/environmentalists-who-changed--and-continue-to-change--the-world">Environmentalists Who Changed (and Continue to Change) the World</a>
<br>
<a href="https://www.discovery.com/nature/first-dog-in-the-us-tests-positive-for-coronavirus">First Dog in the US Tests Positive for Coronavirus</a>
<br>
<a href="https://www.google.com">google</a>
<br>
<a href="https://www.musinsa.com">무신사</a>
<br>
<a href="https://www.nature.com/articles/s41467-020-19623-x">Associations between blood type and COVID-19 infection, intubation, and death</a>
<br>
<a href="https://naver.com">네이버</a>
<br>
<a href="https://www.epost.go.kr/main.retrieveMainPage.comm">우체국 홈페이지</a>
<br>
<a href="https://www.scope.org.uk">스코프 홈페이지</a>
<br>
<a href="https://www.w3.org">W3C 홈페이지</a>
<br>
<a href="https://inviqa.com/blog/web-accessibility-examples-5-sites-doing-it-right">Web accessibility examples: 5 sites doing it right</a>

</details>