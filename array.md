# TIL_HTML-CSS-Javascript

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
<script>
	function choiceAngel(){
		var arr = document.frm.angel;
		//alert(arr.length);
		
		/*
		 * 하나라도 선택하지 않았으면 ...한명의 이상형을 선택하라는 alert 띄우고
		 * 하나이상 선택했으면 ...선택한 이상형을 alert창으로 출력
		 */
		
		var str = "";
		for(var i=0; i<arr.length; i++){
			if(arr[i].checked){//선택한 데이터}
				str+=arr[i].value+" ";
			}//if
			
			arr[i].checked = false;
		}
		 if(str=="") alert("이상형 하나는 선택해주세요!!");
		 else alert("당신의 이상형은 "+str+" 입니다.");
	}

</script>
</head>
<body>
<form name="frm">
	<strong>이상형 선택(중복 선택 가능)</strong><br><br>
	<input type="checkbox" name="angel" value="아이유">아이유<br>
	<input type="checkbox" name="angel" value="김민경">김민경<br>
	<input type="checkbox" name="angel" value="박세리">박세리<br>
	<input type="checkbox" name="angel" value="김소연">김소연<br>
	<input type="checkbox" name="angel" value="현아">현아<br>
	<input type="button" value="choice" onclick="choiceAngel()">
</form>
</body>
</html>
