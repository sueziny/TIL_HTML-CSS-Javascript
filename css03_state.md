# TIL_HTML-CSS-Javascript

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
<style type="text/css">
	/*input:disabled{background:gray;}*/
	
	input[disabled=disabled]{background:gray;}

</style>
</head>
<body>
<h2>State Attribute</h2>
<form>
	<h3>Enabled</h3>
	<input />
	
	<h3>Enabled</h3>
	<input disabled="disabled"/>
	
	<h3>Enabled</h3>
	<input readonly="readonly"/>
	
	<h3>Enabled</h3>
	<input required="required"/>

</form>
</body>
</html>
