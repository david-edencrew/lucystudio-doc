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
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 확장가능한 선택되었던 Style 위젯의 히스토리 목록이 나타납니다.


#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3. 선택 가능한 위젯
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 확장가능한 선택 가능한 Style 위젯목록이 나타납니다.

#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4. 선택하신 위젯
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 선택하신 위젯목록이 나타납니다.


#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 5. + (플러스)
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 선택하신 위젯목록이 나타납니다.(똑같은 위젯으로 중복 가능합니다.)