# action bar 

action bar는 Lucy Studio 상단에 있습니다.
프로젝트 경로, Stage Transition, Git, Bug Viewer, Run, Device Sync, 설정, Profile의 정보를 제공합니다.


![](../../assets/action_bar/action_bar.png)


<br />
<br />
<br />

### 1. 프로적트 경로

현재 개발하고 있는 프로젝트의 경로 디렉토리가 표시 됩니다.

<br />
<br />
<br />

### 2. Canvas Area

Canvas 영역에서 위젯들의 배치 또는 스크립트를 통해서 화면을 그리는 영역을 담당합니다.

![](../../assets/action_bar/canvas_area.png)

<br />
<br />
<br />

### 3. State Transition

화면에서 위젯의 애니메이션 효과를 추가, 또는 변경을 할 수 있습니다.  

![](../../assets/action_bar/st.png)


### 4. Git

오픈소스에서 제공하는 git의 형상관리 툴이 Lucy Studio에 내장되어 있습니다.
기 제공하는 Git가 같은 기능을 제공합니다.

<참고1>
![](../../assets/action_bar/git.png)

<br />

<참고2>
![](../../assets/action_bar/git2.png)

<참고3>
![](../../assets/action_bar/git3.png)

<참고4>
![](../../assets/action_bar/git4.png)

<참고5>
![](../../assets/action_bar/git5.png)

#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1. Unstaged files
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 로컬 저장소에서 작업한 작업 내역이 표시됩니다.


#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2. Staged files
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 서버 저장소에 적용할 작업 내역입니다.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(ex) Unstaged files 체크박스를 클릭 시 위 <9번>항목으로 이동합니다.


#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3. History 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 원격저장소에서 여러 팀원이 작업한 내역을 표시합니다.

#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4. Commit
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Staged files에 지정된 목록을 커밋 기록을 적용하기 위한 단계입니다.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(ex) Commit 클릭 시 <10번>항목의 팝업이 나타나며 코멘트 필수 입력 후에 Commit 버튼을
클릭하시면 커밋 기록에 저장됩니다.


#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 5. Pull
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 원격저장소에 저장되어 있는 파일 목록을 로컬저장소와 동기화를 적용합니다.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Pull버튼을 클릭하시면 <참고5>의 원격저장소와 로컬저장소의 동기화가 이루어 집니다.

#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 6. Push
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;새롭게 생성한 원격 리포지토리에 기존 커밋 기록을 옮기거나, 기존 원격 리포지토리에서 일부 변경된 내용을 옮기는데 사용할 수 있습니다. 

#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 7. Fetch
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 로컬 Git에게 원격 저장소에서 최신 메타데이터 정보를 확인하라는 명령을 전달합니다.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;단 fetch 는 원격 저장소에 변경사항이 있는지 확인만 하고, 변경된 데이터를 로컬 Git에 실제로 가져오지는 않습니다.


#### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 8. Close
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 해당 윈도우창을 닫습니다. 