# greenwireless.github.io

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>Rotating Page</title>
<style type="text/css">
* {
	margin:0;
	padding:0;
	border:0;
}
html, body, iframe {
	height:100%;
	width:100%;
	overflow:hidden;
}
</style>
<script type="text/javascript">
var pages = new Array(); // this will hold your pages
pages[0] = 'page1.html';
pages[1] = 'page2.html';
pages[2] = 'page3.html';
pages[3] = 'page4.html';
pages[4] = 'page5.html';
pages[5] = 'page6.html';

var time = 30; // set this to the time you want it to rotate in seconds

// do not edit
var i = 1;
function setPage()
{
	if(i == pages.length)
	{
		i = 0;	
	}
	document.getElementById('holder').setAttribute('src',pages[i]);
	i++;
}
setInterval("setPage()",time * 1000);
// do not edit
</script>
</head>

<body>
<iframe id="holder" src="page1.html" frameborder="0" scrolling="no"></iframe>
</body>
</html>
