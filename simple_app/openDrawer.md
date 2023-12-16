# openDrawer
화면 A 에서 화면 B 를 엽니다. 화면의 좌측, 혹은 우측에서 새로운 화면이 뜹니다. <br/> 
먼저 페이지 A에서 해당 액션을 잡아둡니다.
<br/><br/> 

현재 경로를 확인합니다. Manual 폴더에 열게될 파일이 저장되어있습니다.<br/> 
현재 페이지 : mainPage <br/>
열리는 페이지 : firstPage

위치를 기본위치에서 Manual 폴더를 만들어서 넣기로 합니다.<br/>
전체 경로를 지정한 위치, 페이지명은 Manual/firstPage 입니다.

"Drawer is left show " 활성화로 왼쪽에서 오른쪽으로 혹은 반대로 동작합니다.
<br/><br/> 
><img src="../assets/ManualCommon/openDrawer1.gif"  width="100%"  height="100%"/>
<br/><br/>


<br/><br/><br/>
이미지를 선택하면 새로운 창이 열리는 액션을 실행하기 위한 이벤트를 입력합니다. <br/>
먼저 이미지를 선택후 Style 에서 "GestureDetector" 를 선택합니다. <br/>
onTap 을 선택해서 이미 만들어둔 액션 "OpenDrawer" 를 선택합니다.
<br/><br/> 
><img src="../assets/ManualCommon/openDrawer2.gif"  width="100%"  height="100%"/>
<br/><br/>
