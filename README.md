# wplab

WEB PROGRAMMING LAB MANUAL
5TH SEM BCA
1. Create an XHTML page that provides information about your department. Your
XHTML page must use the following tags:
a. Text formatting tags
b. Horizontal rule
c. Meta element
d. Links
e. Images
f. Tables
Index.html
<html>
<head>
<meta name="BCA" content="Bachelor of computer applications">
<title>BCA DEPARTMENT</title>
</head>
<body>
<center><h1>Welcome to Presidency Collge(Autonomous)</center></h1>
<hr><br><br>
<table align="center" border="1" cellpadding="10">
<tr>
<td><ol>
<li><a href="aboutbca.html" ><input type="button" vspace="8" hspace="10"
value="ABOUT BCA" /></a></li><br />
<li><a href="fac.html" ><input type="button" vspace="8" hspace="10"
value="FACULTY" /></a></li><br />
<li><a href="croom.html"><input type="button" vspace="8" hspace="10"
value="CLASS ROOM" /></a></li><br />
</td>
<td align="center">
<p>
<img src="2.jpeg" width="500" height="200" align="center" />
</p>
</td>
<td align="center" width="20%">
<img src="3.jpeg" width="200" height="200" align="center"/>
</td>
</tr>
<tr>
<td>
<h2> contact persons</h2>
Dr. SUCHITHRA (Principal)
33/2C and 33/2D, Vinayakanagar, Hebbal Kempapura,
<br> Bangalore – 560024, Karnataka, India
</td>
<td align="center">
<p><pre>
<h2> Department of Computer Application, <br>which started in the year 2000,<br>
offers both BCA and MCA with excellent<br> academic and placement records.
</h2></pre>
</p>
</td>
</tr>
</table>
</body>
</html>
Aboutbca.html
<html>
<head>
<title>ABOUT BCA</title>
</head>
<body>
<center>
<h1> ABOUT BCA</h1>
<per>
“BCA (Bachelor of Computer Applications) is a professional
degree in computer science.
It focuses on providing a theoretical as well as practical
training to students in the related field.”
</per>
</center>
<body>
</body>
</html>
croom.html
<html>
<head>
<title>class room</title>
</head>
<body>
<table align="center" cellpadding="15" border="1">
<caption><h1> CLASSS ROOM </h1></caption>
<tr>
<th>SN</th>
<th>ROOM TYPE</th>
<th>ROOM NUM</th>
<th>SEATING CAPACITY</th>
</tr>
<tr>
<td>1.</td>
<td>class room</td>
<td>B11</td>
<td>lecture room</td>
</tr>
<td>2.</td>
<td>class room</td>
<td>B10</td>
<td>lecture room</td>
</tr>
<td>3.</td>
<td>class room</td>
<td>B6</td>
<td>lecture room</td>
</tr>
</tr>
</table>
</body>
</html>
faculty.html
<html>
<head>
<title>FACULTY LIST</title>
</head>
<body>
<table cellpadding="15" border="1" align="center">
<caption><h1> DCA DEPT. FACULTY LIST</h1></caption>
<tr>
<th>
<b> SN </b>
</th>
<th>
<b> NAME </b>
</th><th>
<b> QUALIFICATION</b>
</th>
<th>
<b> DESIGNATION </b>
</th>
</tr>
<tr>
<td>1.</td>
<td>DR.ALLI</td>
<td>MCA,MPHIL,PHD</td>
<td>HOD</td>
</tr>
<tr>
<td>2.</td>
<td>DR.SHEETAL</td>
<td>MTECH,PHD</td>
<td>PROFF</td>
</tr>
<td>3.</td>
<td>MS ANITHA</td>
<td>MCA,MPHIL</td>
<td>PROFF</td>
</tr>
</tr>
</table>
</body>
</html>
2. Develop and demonstrate a HTML5 page which contains
a) Dynamic Progressive bar.
b) Display Video file using HTML5 video tag.
2a.html
<!DOCTYPE html>
<html>
<style>
#progress_status{
width:50%;
background-color:red;
}
#myprogressBar{
width:2%;
height:20px;
background-color:green;
}
</style>
<body>
<h3>example of progress bar using javascript</h3>
<p> download status of file</p>
<div id="progress_status">
<div id="myprogressBar"></div>
</div>
<br>
<button onclick="update()">start download</button>
<script>
function update(){
var element=document.getElementById("myprogressBar");
var width=1;
var identity=setInterval(scene,10);
function scene(){
if(width>=100){
clearInterval(identity);
}
else{
width++;
element.style.width=width+'%';
}
}
}
</script>
</body>
</html>
2b.html
<!DOCTYPE html>
<html lang="en">
<head>
<title>Document</title>
</head>
<body>
<video width="320" height="240" controls>
<source src="movie.mp4" type="video/mp4">
Your browser does not support the video element. Kindly update it to latest
version.
</video>
</body>
</html>
3. Develop and demonstrate the usage of inline, external and internal style sheet
using CSS. Use XHTML page that contains at least three paragraphs of text, listed
elements and a table with four rows and four columns.
3a.html
<?xml version ="1.0" encoding="utf-8" ?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.2//EN"
"htpp://www.w3.org/TR/xhtml11.DTD/xhtml11.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<html>
<head>
<title>
demonstration of css
</title>
<link rel="stylesheet" href="style.css">
<style>
h3
{
font-family:Garamond;
color:red;
}
</style>
</head>
<body>
<h1><center>Demonstration os CSS - internal,inline and external style
sheet</h1></center>
<h3><u>unix programing</u></h3>
<p style="font-family:verdana;font-size:20pt;color:blue">on 1969 unix programing is
developed by ken Thompson and dennis ritche, unix is a OP which handle all accept of
multiple user and multiple task at a time</p>
<h3>Web Programming</h3>
<p>in 1995, Netscape introduced a client-side scripting language called javascript
following program to add some dynamic elements.</p>
<h3>Software Engineering</h3>
<p>When the first digital computer appeared in the early 1940, the instruction to make
them operate were wired into the machine.</p>
<h3>Student DataBase</h3>
<table border="3" bordercolor="blue" align="center" frame="vsides"
bgcolor="15dksb">
<tr>
<th>regno</th>
<th>name</th>
<th>class</th>
<th>percentage</th>
</tr>
<tr>
<td>15dksb7123</td>
<td>theerthesh</td>
<td>BCA</td>
<td>75%</td>
</tr>
<tr>
<td>15dksb7124</td>
<td>abbas</td>
<td>BCA</td>
<td>73%</td>
</tr>
</table>
</body>
</html>
Style.css
body {
color: blue;
}
p {
color: rgb(11, 10, 21);
font-size: 30px;
font-style: bold;
}
4. Create a XHTML document that describes the form for taking orders for popcorn. Text
boxes are used at the top of the form to collect the buyer’s name and address. These
are placed in a borderless table to force the text box align vertically. A second table
to collect actual order. Each row of this table names a product, displays the price, and
uses text box with size 2 to collect the quantity ordered using <td> tag. The payment
method is input by the user through one of four radio buttons. Provide provision for
submission of order and clear the order form.
4a.html
<html>
<head>
<title> Orders for Popcorn </title>
</head>
<body>
<h1> URBAN PLATTER - Popcorn Sales</h1>
<form>
<table>
<tr>
<td><b> Buyer's Name:</td></b>
<td><input type="text"/></td><br />
</tr>
<tr>
<td><b> Street Address:</td></b>
<td><input type="text"/></td><br />
</tr>
<tr>
<td><b>City, State, Zipcode:</td></b>
<td><input type="text"/></td><br />
</tr>
</table><table border="2">
<th>Product Name</th>
<th>Price</th>
<th>Quantity</th>
</tr>
<tr>
<td> Unpopped Popcorn(100 grams)</td>
<td>&#8377;30.00</td>
<td><input type="text" size="2"/></td>
</tr>
<tr>
<td> Caramel Popcorn(200 grams)</td>
<td>&#8377;35.00</td>
<td><input type="text" size="2"/></td>
</tr>
<tr>
<td> Caramel Nut Popcorn(200 grams)</td>
<td>&#8377;45.00</td>
<td><input type="text" size="2"/></td>
</tr>
</table>
<h2><b>Payment Method:</b></h2>
<input type="radio" name="s"/>Visa
<input type="radio" name="s"/>Master Card
<input type="radio" name="s"/>Discover
<input type="radio" name="s"/>Check
<br>
</br>
<input type="submit" value=Submit Order"/>
<input type="reset" value=Clear Order Form"/>
</form>
</body>
</html>
5. Develop and demonstrate, using JavaScript script, a XHTML document that contains
three short paragraphs of text, stacked on top of each other, with only enough of
each showing so that the mouse cursor can be placed over some part of them.
When the cursor is placed over the exposed part of any paragraph, it should rise to
the top to become completely visible.
5a.html
<html>
<head>Stack Ordering
<title>Stack Ordering</title>
<style type="text/css">
#layer1
{
border:solid thick black;
background-color:brown;
padding:10px;
width:300px;
height:200px;
position:absolute;
top:100px;
left:200px;
z-index:0;
}
#layer2
{
border:solid thick black;
background-color:gray;
padding:10px;
width:300px;
height:200px;
position:absolute;
top:120px;
left:220px;
z-index:0;
}
#layer3
{
border:solid thick black;
background-color:white;
padding:10px;
width:300px;
height:200px;
position:absolute;
top:140px;
left:240px;
z-index:0;
}
</style>
</head>
<body>
<script type=text/javascript>
var topLayer="layer3";
//function to place the choosen layer on the top
function mover(toTop)
{
document.getElementById(topLayer).style.zIndex="0";
document.getElementById(toTop).style.zIndex="1";
topLayer=toTop;
}
</script>
<p id=layer1 onMouseOver=mover('layer1');>This is the last layer</p>
<p id=layer2 onMouseOver=mover('layer2');>This is the middle layer</p>
<p id=layer3 onMouseOver=mover('layer3');>This is the first layer</p>
</body>
</html>
