//HTML 
<!DOCTYPE html> 
<html>
<style>
body {
  background-color: white;
  color: black; 
}
</style>
<body id='object'>
<h2>Day/Night Mode </h2>
<p>ボタンを押すと自動的にDay/Nightモードを設定する。</p>
<button onclick="Change()">Day/Night mode</button>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
</body>
</html>

<script>
//JS 
function Change(){
//関数の設定
 var d = new Date();
 // 日程情報が得られるメソッド new Date()を使う
 var hour = d.getHours();
 var min = d.getMinutes();
 //　それから詳細な時間が得られるメソッドを使う
 if(hour<=17&&hour>7){
 document.getElementById('object').style.backgroundColor = "white"; 
 document.getElementById('object').style.color = "black"; 
 window.alert("現在"+hour+"時"+min+"分なのでDay modeになります");
 } else {
 document.getElementById('object').style.backgroundColor = "black";
 document.getElementById('object').style.color = "white";
 window.alert("現在"+hour+"時"+min+"分なのでNight modeになります");
 } 
 //詳細な時間とday/night modeの判断結果を示す
}
  </script>
