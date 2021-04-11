# TIL_HTML-CSS-Javascript

<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>table에 hover 효과주기</title>
<style type="text/css">
	td{
		text-align:center;
	}
	tfoot{
		background-color:pink;
	}
	/* table에 자식 태그인 tr을 선택자로 지정
	   table tr : table의 후손개념인 tr
	   table>tr : table의 직계자식인 tr
	   
	*/
	table>tbody>tr:hover{
		background-color:yellow;
	}

</style>
</head>
<body>
<h2 align="center">table에 hover 효과 주기</h2>
<table align="center" border="2" width="40%">
	<caption>Table Caption</caption>
	<colgroup>
		<col span="2" style="background:red">
		<col style="background:blue">
	</colgroup>

	<thead>
		<tr>
			<th>NO</th><th>NAME</th><th>ADDR</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td colspan="3">1</td>
		</tr>
		<tr>
			<td>2</td><td>BBB</td><td>TEXAS</td>
		</tr>
		<tr>
			<td>3</td><td>CCC</td><td>Brandon</td>
		</tr>
	</tbody>
	<tfoot style="background:yellow">
		<tr>
			<td>111</td><td>222</td><td>333</td>
		</tr>
	</tfoot>
</table>
</body>
</html>


