# panel tabbar

properties, Styles, Data Source, Provider Instance, CDS, Data Binding, Action 기능을 제공합니다.


![](../../assets/panel_tabbar/panel_tabbar.png)
<br />
<br />
<br />

### 1. Properties
<br />
   
   property는 선택된 위젯의 색상, 폰트크기 등 여러가지 옵션을 변경할 수 있습니다.

<br />

![](../../assets/panel_tabbar/property.png)


<br />
<br />
<br />

* Data Binding
    1. Provider를 통해서 연동 된 데이터셋을 Provider Instance로 생성합니다.
    2. 생성 된 Provider Instance를 Data Source와 연동합니다.
    3. 연동 된 Data Source와 위젯의 고유 ID를 통해서 위젯의 값 또는 옵션 등의 연결을 지원합니다.  

<br />

![](../../assets/panel_tabbar/databinding.png)

<br />
<br />
<br />

### 2. Styles
<br />
 
선텍하신 위젯의 확장기능으로 SizedBox(크기변경), Padding(여백조절)등등 여러가지 옵션으로 멀티로 추가가 가능하며 
원하시는 디자인에 최적화가 가능합니다. 

<br />

![](../../assets/panel_tabbar/styles.png)

<br />

#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1. 검색
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 확장가능한 Style 위젯의 검색이 가능합니다.


#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2. Recently
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 추가한 Style 위젯의 히스토리 목록이 나타납니다.


#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3. 추가 가능한 위젯
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 확장가능한 선택 가능한 Style 위젯목록이 나타납니다.

#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4. 추가 된 위젯
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 추가한 위젯목록이 나타납니다.


#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 5. + (플러스)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 선택하신 위젯의 위,아래에 Style 위젯 추가가 가능합니다.(동일 위젯으로 중복 사용 가능합니다.)


### 3. Data Source
<br />

서버에 정의되어 있는 데이터 정보를 설정해서 필요한 필드정보를 가져올 수 있습니다. 

<첨부1>

![](../../assets/panel_tabbar/ds1.png)


<첨부2>

![](../../assets/panel_tabbar/ds2.png)

<첨부3>

![](../../assets/panel_tabbar/ds3.png)

<첨부4>

![](../../assets/panel_tabbar/ds4.png)

<첨부5>

![](../../assets/panel_tabbar/ds5.png)


<br />
<br />

 
> Data Source를 추가하기 위해서 다음과 같이 설정하시면 됩니다.
>
> 
> 1.  (+) 버튼을 클릭하시면 팝업화면(Create Data Source)창이 나옵니다.
> 2.  필수 입력사항인 Data Soure Name을 입력합니다.
> 3.  비필수 입력사항인 <2번>(Data Soure Name)에 대한 설명이 필요할 경우 사용합니다.
> 4.  서버의 데이터를 가져오기 위해서 입력값 설정이 필요한 경우 Call Defination를 사용하시면 됩니다.
> 5.  서버의 데이터를 가져오기 위해서 출력값 설정이 필요한 경우 아래 <12번>화면 Response Definition에서 필드 정보를 설정하시면 됩니다.
> 6.  Add Group를 클릭 시 아래 빨간색 라인이 필드가 추가되며 데이터의 입력값이 List형태인 경우 체크박스를 설정할 수 있습니다.
> 7.  Add Field를 클릭 시 아래 파란색 라인이 필드가 추가되며 필드명, 데이터 타입, 주석입력이 가능합니다.
> 8.  Load Provider Instance를 클릭하시면 우측화면에 설정하셨던 Provider Instance 데이터 목록이 보입니다.(<첨부4> 이미지 참조)
> 9.  추후 설명
> 10. Save 버튼을 클릭 시 Data Source 데이터 목록에 <첨부2>와 같이 추가됩니다.
> 11. Data Source를 추가하실 경우 <첨부2>와 같이 표시됩니다.
> 12. <4번>과 같이 동일한 방법으로 아웃풋 필드정보 설정이 가능합니다. 
> 13. Provider Instance로 설정한 데이터셋 목록 중에서 E1413를 더블 클릭 시에 E1413(Provider)에 설정한 원본 데이터셋이 복사됩니다.(<첨부5>의 <14번> 참조)
> <br />
>





