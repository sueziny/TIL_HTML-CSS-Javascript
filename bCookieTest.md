# TIL_HTML-CSS-Javascript

<%@ page language="java" contentType="text/html; charset=UTF-8"
    pageEncoding="UTF-8"%>
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
</head>
<body>
<h2>ACookieTest에서 저장된 쿠키 정보를 받아옵니다...</h2>
<%
	Cookie[ ] cs=request.getCookies();
	for(Cookie c : cs){
		out.println(c.getName()+"-------"+c.getValue()+"<br>");
	}

%>
</body>
</html>
