# vinay-codes
1.)  HTML and CSS program for text shrinking and text glowing.



<!DOCTYPE html>
<html>
<head>
<style>
p
{
 position:absolute;
 top:50%;
left:50%;
transform:translate(-50%,-50%);
}
</style>
</head>
<body>
<p id="demo"></p>
<script>
 var var1 = setInterval(inTimer,500);
var fs = 5;
var ids = document.getElementById("demo");
function inTimer()
{
ids.innerHTML = "TEXT GROWING";
ids.setAttribute('style',"font-size: " + fs + "px; color: red");

fs +=5;
if(fs >=50)
{
clearInterval(var1);
var2 = setInterval(deTimer,500);

}
}
function deTimer()
{
fs -= 5;
ids.innerHTML = "Text SHRINKING";
ids.setAttribute('style', "font-size: " + fs + "px; color: blue");
if(fs == 5)
{
clearInterval(var2);

var1 = setInterval(inTimer,500);
}
}
</script>
</body>
</html>

