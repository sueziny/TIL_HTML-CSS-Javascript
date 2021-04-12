# TIL_HTML-CSS-Javascript

<!DOCTYPE html>
<html>
<head>
<meta charset="EUC-KR">
<title>Insert title here</title>
<style>
	.box{
		width: 150px;
		height: 150px;
		background: #cccccc;
		float: left;
		margin-right: 10px;
	}
	.vi{ overflow: visible;}
	.hi{ overflow: hidden;}
	.sc{ overflow: scroll;}
	.au{ overflow: auto;}
	
	
	/* .vi h3{ color: red;	} */
	
	.vi>h3{ color: red;	}
</style>
</head>
<body>
 	<div class="box vi">
      <h3>visible::직계자식입니다.</h3>
      <div>
      	 <h3>후손입니다..</h3>
      </div>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean nec mollis nulla. Phasellus lacinia tempus mauris eu laoreet.</p>
    </div>
    <div class="box hi">
      <h3>hidden</h3>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean nec mollis nulla. Phasellus lacinia tempus mauris eu laoreet.</p>
    </div>
    <div class="box sc">
      <h3>scroll</h3>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean nec mollis nulla. Phasellus lacinia tempus mauris eu laoreet.</p>
    </div>
    <div class="box au">
      <h3>auto</h3>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean nec mollis nulla. Phasellus lacinia tempus mauris eu laoreet.</p>
    </div>
</body>
</html>
