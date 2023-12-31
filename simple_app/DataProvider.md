# Data Provider 등록

통신을 위한 연결부터 실행한다. 서버에 연결하며 네트워크 담담자에게 해당 정보를 문의한다.

최초에는 접속할 서버정보를 셋팅해야한다.<br/>
[서버접속참조](/simple_app/Communication.md)
<br/>


![](<../assets/simple_app/dataprovider01.png>)

1. Data Provider Panel 에서 새로운 세션을 만든다.
2. 신규 세션을 생성한다. 
3. 위 화면은 “jongmok” , “memus” 라는 세션을 이미 만든상태를 보여준다. 
4. 연필모양을 눌러서 수정이 가능하다.
5. 지금 할 테스트는 json 파일에서 정보를 읽어와서 화면에 보여주는 것으로 해당 json 파일의 구조 및 이름이 같아야한다. 

<br />
<br />
<br />


## 샘플 생성 및 등록
- 샘플은 파일을 읽어 화면에 데이터를 보여주는 작업을 보여준다. 먼저 내부설정부터 아래와 같이 작업한다.
  
![](<../assets/simple_app/dataprovider02.png>)

<br/>

1. Call Definition 영역에서 (사용자가 input 데이터를 넣는 영역)
2. 먼저 DataProvider 이름을 정하고 엔터
3. 타입은 수동타입인 "Custom" 선택한다.
4. 분석 타입은 "json" 을 선택한다.

<br/><br/><br/>

![](<../assets/simple_app/dataprovider03.png>)
<br/>

1. Response Definition 영역에서 (읽어서 가져올 데이터 영역)
2. 그룹을 추가한다. 그룹의 이름은 jongmok.json 파일의 outBlock0 이름과 같아야 한다.
<br/> (아래의 jongmok.json 샘플참조)
3. 그룹 “outBlock0”를 선택후 필드를 추가한다. (그룹내에 배열 데이터들을 추가하기위함)
4. 나머지 필드들 title, name, price, gap, rate 등의 필드들도 Group 아래에 추가한다. 반드시 이름이 같아야한다.
<br/> (아래의 jongmok.json 샘플참조)

<br/><br/><br/>

![](<../assets/simple_app/dataprovider04.png>)
<br/>

5. 추가이후  “outBlock0”의 앞 화살표를 선택시에 위와같이 접히는 구조가 되어야 정상이다.
6. Data Provider 설정의 완료는 여기까지 이며 이후의 작업은 ProvInstance 등록 과정으로 연결된다. 

   [ProvInstance 등록과정](/simple_app/Communication.md)

<br/><br/><br/><br/><br/><br/><br/><br/><br/>

샘플데이터 : `jongmok.json` 의 구조 및 데이터 
<br/>

1. 아래 텍스트를 복사한다.
2. 파일명을 `jongmok.json` 으로 만든다.
3. jongmok.json 저장경로를 LUCY 설치 폴터의 .... 에 저장한다.

<br/>
<br/>

{
    "outBlock0" :
    [
        {
            "title" : "ROTI",
            "name" : "Nippon Indosari Tbk",
            "price" : "8600",
            "gap" : "+50",
            "rate" : "+3.23%"
        },
        {
            "title" : "GOTO",
            "name" : "GoTo Gojek Tokopedia",
            "price" : "2421",
            "gap" : "-121",
            "rate" : "-20.6%"
        },
        {
            "title" : "ABNB",
            "name" : "Airbnb Inc",
            "price" : "5300",
            "gap" : "+31",
            "rate" : "+2.23%"
        },
        {
            "title" : "UNVR",
            "name" : "Unilever Indonesia",
            "price" : "3867",
            "gap" : "-71",
            "rate" : "-41.1%"
        }
    ]
}

