# Data Provider 등록 (LoadFile Action)

통신을 위한 연결부터 실행합니다. 서버에 연결하며 해당정보는 네트워크 담담자에게 문의합니다.

최초에는 접속할 서버정보를 셋팅해야 합니다. <br/>

[1. 최초 서버접속 설정이 완료되어야 합니다.](/simple_app/Communication.md)
<br/>


이후 

![](<../assets/simple_app/dataprovider01.png>)

1. Data Provider Panel 에서 새로운 세션을 만듦니다.
2. 신규 세션을 생성합니다. 
3. 위 화면은 “jongmok” , “memus” 라는 세션을 만들었습니다. 이미 만든상태를 보여줍니다. 
4. Edit 아이콘을 누르면 수정이 가능합니다.
<br />
<br />
<br />
<br />   

#### 지금 할 테스트는 json 파일에서 정보를 읽어와서 화면에 보여주는 것입니다. 
#### 이는 해당 json 파일의 목록구조와 Provider 내부의 변수 이름이 같아야 합니다. 
<br />

### 샘플 생성 및 등록
- 샘플은 파일을 읽어 화면에 데이터를 보여주는 작업을 보여줍니다. 먼저 내부설정부터 아래와 같이 설정합니다.
  
![](<../assets/simple_app/dataprovider02.png>)

<br/>

1. Call Definition 영역에서 (사용자가 input 데이터를 넣는 영역)
2. 먼저 DataProvider 이름을 정하고 엔터키를 누릅니다
3. 타입은 수동타입인 "custom" 선택 합니다.
4. 분석 타입은 "json" 을 선택합니다.

<br/><br/><br/>

![](<../assets/simple_app/dataprovider03.png>)
<br/>

1. Response Definition 영역에서 (파일을 읽어서 가져올 데이터 영역)
2. 그룹을 추가합니다. 그룹의 이름은 jongmok.json 파일의 outBlock0 이름과 같게 합니다.
<br/> (아래의 jongmok.json 샘플참조)

3. 그룹 “outBlock0”를 선택후 필드를 추가합니다.
   <br/>  (그룹내에 배열 데이터들을 추가하기 위함입니다)
4. 나머지 필드들 title, name, price, gap, rate 등의 필드들도 Group 아래에 추가합니다. 
<br/> 이때 반드시 이름이 같아야 합니다.(아래의 jongmok.json 샘플참조)

<br/><br/><br/>

![](<../assets/simple_app/dataprovider04.png>)
<br/>

5. 이후 정상적으로 추가가 되었다면 “outBlock0”의 앞 화살표를 선택시에 위와같이 접히는 구조가 되어야 정상입니다.
6. Data Provider 설정의 완료는 여기까지 이며 이후의 작업은 ProvInstance 등록 과정으로 넘어갑니다. 
   
<br/><br/><br/>

   [ProvInstance 등록과정을 보여주는 LoadFile Link](/simple_app/LoadFile.md)

<br/><br/><br/><br/><br/>
