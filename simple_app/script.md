# 현재 자바 스크립트 실행되는 함수 & 변수	


### $act.executeAction( string actionName );

1. 예시 : $act.executeAction("action_coin_detail"); <br/>
     $act.executeAction("E3921_req");  <br/>
 설명 : 액션패널에 (이미 등록되어) 있는 액션을 실행한다.<br/>

<br/>
<br/>

### $vm.loadFileData("piName", "FileName");

1. 예시 : $vm.loadFileData("prov_ins_coin_detail_0", "coin_detail.json"); <br/>
  설명 : Json 파일은 assets/data 폴더에 있어야 한다. <br/>
	     액션항목에서 trigger->loadFile 과 같은 기능을 실행한다.

<br/>
<br/>

### $act.startStateTransition("ST Group ID");

1. 예시 : $act.startStateTransition('bidaskBar_rFront'); <br/>


<br/>
<br/>


### "widget_id".setProperty("Property", "사용값" ); 

이미지 위젯 사용시 : 위젯의 아이디를 "id_img" 을 지정하고  <br/>
1. 예시 : id_img.setProperty("image.assetName", "assets/images/newssource2005.png"); <br/>
설명 : 이미지 위젯의 이미지 명을 지정해준다. <br/>

2. 예시 : id_img.setProperty("image.url", IMG_PATH + sCode +".png"); <br/>
설명 : URL 로 이미지를 지정하는 경우

<br/>
<br/>
텍스트 위젯 사용시 : 위젯의 아이디를 "id_text" 을 지정하고 <br/>

<br/>

1. 예시 : id_text.setProperty("text", "'인플레 공포'에 투심악화... 코스피 2%하락 출발"); <br/>
설명 : 텍스트 위젯의 글자항목에  “인플레…. 출발" 정보를 보여준다.

2. 예시 : id_text.setProperty("style.color", "#EA0C0C"); <br/>
설명 : 텍스트 위젯의 글자에 컬러를 #EA0C0C (빨강)으로 변경한다. 

3. 예시 :  id_text.setProperty("style.fontStyle", "italic"); <br/>
설명 : 텍스트 위젯의 글자에 이탤릭 형을 먹인다.


> 스타일영역의 위젯에 설정값을 변경하기 위해서는 setStyleProperty 를 사용한다.

4. 예시 : id_text.setStyleProperty("DecoratedBox","decoration.color", “#1AF93F62); <br/> 
설명 : 스타일 위젯에서 “F93F62” 컬러와 1A (10%만큼) opacity 를 준다. <br/>

5. 예시 : id.setStyleProperty("DecoratedBox","decoration.color",bg_color); <br/>
설명 : 스타일 위젯에서  "bg_color" 변수의 값을 컬러로 지정한다. <br/>

6. 예시 : id.setStyleProperty("DecoratedBox","decoration.color",setColor(man1, "1A") );  <br/>
설명 : 스타일 위젯에서 함수 "setColor" 로 리턴된 값을 지정한다. <br/>

8. 예시 : id.setStyleProperty("SizedBox","width", Math.abs(man2/man1)*230 ); <br/>
설명 : 스타일 위젯에서 사이즈박스를 주는데 그 넓이는 "Math.abs(man2/man1)*230" 이것만금 준다. <br/>

<br/><br/>


## 화면 띄우기, 팝업, 등등

### $app.openBackPage();
1. 예시 : $app.openBackPage(); <br/>
설명 : 이전 페이지로 돌아간다. 현재페이지는 삭제함. 이전페이지가 다시보여짐

### $app.openPage( string pagePath, string route );
1. 예시 : $app.openPage('invest_info/stock_kor', {code: inCode}); <br/>
설명 : 새로운 페이지를 연다. 열리는 페이지명은 invest_info/stock_kor 이며, 넘겨줄 인자로 code값을 넘겨준다. <br/>
넘겨준 인자는 새로 열리는 페이지의 onStart 함수에서 받으며 예시는 key:value 방식으로 받는다. 

2. 예시 : $app.openPage('invest_info/stock_kor', code); <br/>
   설명 : 새로운 페이지를 연다. 위와 같으나 넘겨주는 인자는 code 이다.


### $form.openDrawer( string formPath, bool isStartPos );
좌측 혹은 우측에서 화면 띄우기

### $form.openSheet (string formPath, bool isModal );
아래에서 화면 띄우기

### $form.navigatorPop( );
현재 페이지를 스택에서 제거할 수 있습니다.

### $form.openDialog( string formPath );




### $vm.getDataCount(“ContentsDS”);
예시 : 

    let cnt = $vm.getDataCount("E4100_ds.responsePack.E4100OutBlock");
    if(cnt == 0)  {
      id_news_listview1.visible = false;
      id_nodata_col.visible = true;
    }

설명 : 컨텐츠 CDS에 들어온 데이터의 수를 얻는다. 



Iterator Objet

Int add();
void insert ( int index );
void remove (int index );
void clear ();
void setState(int index, JSfunction function);

Setters
Int count();
Int current();
Int selected();

Getters
Int count();
Int current();
Int selected();

TextObjet

void setText(string s );
void setTextSize (double size);
void setTextRGBColor( int R, int G, int B);


아래 위젯들은, 주신내용은 아직 없음.
ListViewObjet
TextFieldObjet
ChartObjet





현재 동작
onStart ();
    form 이 열릴때 바로 실행한다. 해당 함수내에 다른 스크립트를 넣어서 사용한다. 
    사용예 : function onStart() { … … }



### onActive
1. 예시 : 
---
    function onActive() {
        $act.executeAction("IVMGWAREQ01_tr");  
    } 
설명 : 다른 화면으로 넘어갔다가(openPage) 이후 다시 되돌아 올때 (본 화면이 활성화될때) 동작한다. 


### onRequestBefore(provInstName);
1. 예시 :
---
    function onRequestBefore(piName) {
        if("E3511_0" == piName) 
        { 
            let sInBlock = "DS_E3511.callPack.E3511InBlock0.";
            $vm.setDSValue(sInBlock + "act_noz11", _accInfo.sAccNo  );     //  걔좌번호
            $vm.setDSValue(sInBlock + "pswd_no_gbz1", "E"  );              // 운영에서는 S 로 세팅
            $vm.setDSValue(sInBlock + "pswd_noz300", _accInfo.sAccPWD);    //  걔좌비밀번호
        }
        if (piName == "E1611_0")  {
            let gubun = $vm.getFieldData("chart_ds.callPack.inBlock0.gubun"); 
        }
    }
설명 : ProvInstance 서비스를 요청하기전에 무언가를 설정하기 위한  함수. 보통 Key 값을 셋팅하기 전에 사용된다


### onRequestAfter(provInstName);

### onReceiveError(provInstName);



### onResponseUpdateBefore(dsName, piName)
1. 예시 : function onResponseUpdateBefore (dsName, piName) <br/>
설명 : provInst 서비스 요청후 CDS에 업데이트 한후 , 그리고 위젯에 셋팅하기 전에 뭔가를 하기 위한 함수

2. 예시 : <br/>
 --- 
     function onResponseUpdateBefore (dsName, piName)
    {
        if (piName == "E3511_0") 
        {
            if(_isFirst == true) {
                drop_sort.setProperty("value", "1"); // 버튼 초기화      
                        
                // 최초에 1번 수익률로 sort 한다. Sort는 Before 단계에서 DS를 정렬하게 되면 
                // 바뀐 Sort 순서대로 DS에 데이터가 채워지게 된다.       
                $vm.sortNumber("DS_E3511", "E3511OutBlock1.pft_rtz15" , "descending");
                
                _isFirst = false;
            }
        }
    }

설명 : 위젯에 데이터를 넣기 전에 해당 DS를 정렬한후 데이터는 위젯에 들어가게된다. 

### onResponseUpdateAfter (dsName, piName);
1. 예시 : function onResponseUpdateAfter (dsName, piName) <br/>
설명 : provInst 서비스 요청후 CDS에 업데이트 한후 , 그리고 위젯에 셋팅을 한 후에 뭔가를 하기 위한 함수

2. 예시 :   
---
    function onResponseUpdateAfter (dsName, piName) {
        if (piName == "E3511_0") {
            $act.executeAction("IVMGWAREQ01_tr");    
        }
    }
설명 : 데이터를 조회한후에 다음의 액션(이후에 발생할 TR)을 실행한다. 


### onPushUpdateBefore(dsName, piName);


### onPushUpdateAfter(dsName, piName);
1. 예시 :
---
    function onPushUpdateAfter(dsName, piName) {
            
        if(dsName == "DS_E3511") {
            // 현재가가 새로 들어왔다. 계산하자. 
            let Cal_ds = CalcPosDsData(ds, item);
        }
    }
설명 : 실시간 데이터 받은뒤에 이벤트를 처리한다. CDS에 데이터를 올린뒤에 이벤트를 처리한다.


2. 예시 :
---
    function onPushUpdateAfter (dsName, piName) {
        if(dsName == "E1110_ds") 
        {
            showBidAskArrow();

            let volpcolor = $vm.getDSValue("E1110_ds.responsePack.OutBlock.volpower");
            if(parseFloat(volpcolor) > 100)
                bg_color     = "#F93F62"; // bg color        
            else                
                bg_color     = "#4780FF"; // bg color   
            id_volpower.setProperty("deerColor",bg_color);
        }
    }



### Log(); 

사용예시
1. Log.i(“Info  로그입니다.”); <br/>
2. Log.e(“Error 로그입니다. 현재시간 : “ + Date() ); <br/>
3. Log.d(“Debug 로그입니다.arg code: “ + arg.code );  <br/>
설명 : 루시 캔버스 창에는 하단에 Console, Packet 창이 있다. 이중 Packet 창에 로그를 남긴다. <br/>
i, e, d 등의 차이는 로그창에 색상으로 구분된다.



$form.openModalSheet(PageName.FormName); 

설명 : 폼파일을 모달(아래에서 위로)형태로 연다.

$form.openModalSheet("login/auth_4.auth4"); 
“login 폴더내에 있는 auth_4 페이지 파일내의 auth4 라는 폼을 연다.




$vm.getProviderData(piName + ".responsePack.IVMNEWREQ01Out[2].code")

설명 : 얻고자하는 필드명의 데이터를 읽어온다. 

사용예시
let recv=$vm.getProviderData(piName + ".responsePack.IVMNEWREQ01Out[2].code");
$log.d("recvVal = " + piName + "ㅁㅁ" + recv);

수신한(responsePack) 데이터의 3번째 배열(“IVMNEWREQ01Out[2]”)의 code 을 가져온다.



let recvPath = $vm.evalProviderJsonPath(piName + ".responsePack", "$.IVMNEWREQ01Out[*].hts_kor_isnm")

설명 : 배열의 일부분 변수의 값을 배열형태로 가져온다. 가져올땐 JSON 타입으로 가져옴.

사용예시
let recvPath = $vm.evalProviderJsonPath(piName + ".responsePack", "$.IVMNEWREQ01Out[*].hts_kor_isnm");
$log.d("recv path val = " + JSON.stringify(recvPath));

수신한(responsePack) 배열데이터에서 모든블럭(0~n)의 hts_kor_isnm 데이터를 가져온다.



$vm.insertDSValue("bookData.responsePack.Block0[1]", {“key”:”value”, …  } 

설명 : 수신한 DS데이터에서 데이터를 추가(insert)한다.
실제로 listView 위젯에 데이터가 추가된다.



$vm.appendDSValue("bookData.responsePack.Block0", {“key”:”value”, … })

설명 : 수신한 DS데이터에서 데이터의 추가(append)한다.
실제로 listView 위젯에 데이터가 추가된다.



$vm.setDSValue("bookData.responsePack.Block0[1]", {“key”:”value”, … })

설명 : 수신한 DS데이터에서 데이터를 추가(insert)한다.
실제로 listView 위젯에 데이터가 추가된다. 이건 replace 개념

예를들어
$vm.setDSValue("bookData.responsePack.Block0[1]", 
{"time":"000660", "price":"10900", "name":"하이닉스"})

기존에 필드의 전체내용이 time, price, sign, change, name 이었다면 
위에 예시의 setDSValue 를 통해서는  
나머지 필드 sign, change, 들은 없어짐, 이럴땐 전체 DS 에 맞게 추가를 해줘야함. 



setStyledText(
[
{	
text : "안녕",
color: "#0000FF"    
},
{
text: "!!!",
italic:true
}
]
)


setStyledText([
{
text : "abc ABC 이건 두껍께",
weight: "900",
size: 12,
color: "Tertiary",
fontFamily: "Courier",
},
{
text: "!!!", 
italic:true, 
underLine:true, 
weight:"200",      
backColor: "#7700FFFF",                
}])
 

setStyledText(
{
text : "abc 단건",
weight: "500",
size: 12,
color: "Tertiary",
})


clearStyledText();  

setStyledText 사용법은 위와 같다.
설명 : 예시참고

clearStyledText
설명 : 스타일의 삭제, 원래의 데이터는 남는다. 


### $vm.dsUpdateLock(dsName, boolean);
1. 예시 : $vm.dsUpdateLock("DS_E3511", true);
설명 : DS 의 Lock 을 true 상태로 만들어둔다. false로 설정할때 해당 DS의 Lock 이 풀린다.
