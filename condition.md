# TIL_HTML-CSS-Javascript

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
<script>
/* 
입력된 나이가 19세 이상이면 "성인입니다. 사이트 입장 가능" alert창 띄우고
19세 미만이면 "사이트 입장 불가능" alert창 띄우고 
위 작업 모두 진행 한 후, 입력박스의 값을 초기화 시키고, 커서는 다시 위치시킨다.

만약 입력된 값이 없으면 값 입력하라는 메세지 alert창 띄우고 
숫자 대신에 문자 입력시 나이는 숫자로 입력 바란다는 메세지 alert창 띄우고 
*/

function checkAge(){
		//닉네임으로 입력한 값을 하나의 변수에 할당...
		var age = document.agefrm.age;
		if(age.value==""){//값 입력 안했을시}
			alert("나이를 입력하세요");
		}else if(isNaN(age.value)){//isNaN...isNotANumber...문자입력시
			alert("나이는 반드시 숫자로 입력하세요");
		}else if(age.value>=19){
			alert(age.value+" 는 성인 인증...");
		}else{
			alert("미성년자...");
		}
		
		age.value = "";
		age.focus();
	}

</script>
</head>
<body>
<form name="agefrm">
		나이 <input type="text" name="age">
		<input type="button" value="나이확인" onclick="checkAge()">
	</form>
</body>
</html>
