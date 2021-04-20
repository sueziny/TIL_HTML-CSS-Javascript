# TIL_HTML-CSS-Javascript

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
<script>
/* 선언적 함수 선언하기 */
	function showData(){
		//닉네임으로 입력한 값을 하나의 변수에 할당...
		var nickName = document.loginform.nick.value;
		alert(nickName+"Hello");
		document.loginform.nick.value = "";
		document.loginform.hobby.focus();
	}
	function showHobby(){
		var hobby = document.loginform.hobby.value;
		alert(hobby+"Hello");
		document.loginform.hobby.value = "";
	}
</script>
</head>
<body>
	<form name="loginform">
		닉네임 <input type="text" name="nick">
		<input type="button" value="닉네임보기" onclick="showData()" ><br/></br>
		취 미 <input type="text" name="hobby" on>
		<input type="button" value="취미보기" onclick="showHobby()">
	</form>
</body>
</html>
