# TIL_HTML-CSS-Javascript

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>데이터 타입과 선언방법</title>
<!-- 
자바스크립트에서 사용하는 기본 데이터 타입

number
string
boolean
함수형
객체형
undefined
 -->
<script>
	var varialble;
	var stringvar= "String"; //String stringvar = "String";
	var numbervar = 273;
	var booleanvar = true;
	var functionvar = function(){}; //function다음에 함수의 이름이 생략됨. --> 익명함수
	var objectvar = {};//json
	
	/*alert(variable);	
	alert(stringvar);
	alert(numbervar);
	alert(booleanvar);
	alert(functionvar);
	alert(objectvar);*/

	//각각의 값의 데이터 타입(변수타입)을 출력
	alert(typeof variable);	
	alert(typeof stringvar);
	alert(typeof numbervar);
	alert(typeof booleanvar);
	alert(typeof functionvar);
	alert(typeof objectvar);
	
</script>
</head>
<body>

</body>
</html>
