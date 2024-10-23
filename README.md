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




BCA
V SEMESTER
WEB PROGRAMMING LAB
 
Part -B
 
6)Develop a simple calculator to perform arithmetic (addition, subtraction, multiplication and division) operations on given two numbers. Use an html tag that allows the user to input two numbers and to display the result of arithmetic operation. Write suitable HTML and JavaScript and CSS to your simple calculator. The following figure show sample document display.
 
6 Program: -
<html>
    <head>
        <title>input tutorial</title>
        <script lang="javascript">
            function addNumbers(clickedValue)
            {
                var val1=parseInt(document.getElementById("value1").value);
                var val2=parseInt(document.getElementById("value2").value);
                var btnValue = document.getElementById(clickedValue).innerText;
                var andD = document.getElementById('answer')
                if(btnValue=="ADD")
                    document.getElementById("answer").innerText = val1+val2
                else if(btnValue=="SUB")
                    document.getElementById("answer").innerText = val1-val2
                else if(btnValue=="MUL")
                    document.getElementById("answer").innerText = val1*val2
                else if(btnValue=="DIV")
                    document.getElementById("answer").innerText = val1/val2
            }
            function sz()
            {
                document.getElementById("value1").value="";
                document.getElementById("value2").value="";
                document.getElementById("answer").innerText="";
            }
        </script>
    </head>
    <body>
        <center>
            <div style="margin:25vh auto;width:300px;padding:20px;background-color:lightblue;border:5px solid aqua;border-radius:20px;">
                <h2>simple calculator</h2>
                Number 1=<input type="text" id="value1" name="value1" value=""/><br><br>
                Number 2=<input type="text" id="value2" name="value2" value=""/><br><br>
                result = <span id="answer"></span><br><br>
                <button  id="ADD"  onclick="addNumbers('ADD')">ADD</button>
                <button  id="SUB"  onclick="addNumbers('SUB')">SUB</button>
                <button  id="MUL"  onclick="addNumbers('MUL')">MUL</button>
                <button  id="DIV"  onclick="addNumbers('DIV')">DIV</button>
                <button  id="CLEAR" onclick="sz()">CLEAR</button>
            </div>
        </center>
    </body>
</html>
 
 
 
7) Create a web page using two image files, which switch between one another as the mouse pointer moves over the image. Use the on Mouse Over and on Mouse out event handlers.
 
7 Program: -
<!DOCTYPE html>
<html>
<head>
<script>
 
function normalImg() {
  document.getElementById("smile").src = "./smiley.gif"
}
function singing() {
  document.getElementById("smile").src = "./sing.gif"
}
 
</script>
</head>
<body>
 
<img onmouseout="normalImg()" border="0" src="smiley.gif" alt="Smiley" width="300" height="320" id="smile"
onmouseover="singing()" border="0" src="sing.gif" alt="singing" width="300" height="320">
 
<p>onmouse out and onmouseover changing images</p>
 
</body>
</html>
8) Create a form for Student information. Write JavaScript code to find Total, Average, Result and Grade.
 
8 Program: -
<!DOCTYPE html>
<html>
<head>
<title>Registration Form</title>
<script type = "text/javascript">
    function calc()
    {
        var m1,m2,m3,avg = 0,total = 0, result = "",grade = "";
        m1 = parseInt(document.form1.wp.value);
        m2 = parseInt(document.form1.sp.value);
        m3 = parseInt(document.form1.cg.value);
        total = m1+m2+m3;
        avg = total/3;
        if( m1 < 35 || m2 < 35 || m3 < 35)
        {
            result = "fail";
            grade = "D";
        }
        else if(avg >= 75)
        {
            result = "Distinction";
            grade = "A+";
        }
        else if(avg >= 60 && avg < 75)
        {
            result = "First class";
            grade = "A";
        }
        else if(avg >= 50 && avg < 60)
        {
            result = "Second class";
            grade = "B";
        }
        else if(avg >=35 && avg < 50)
        {
            result = "Pass class";
            grade = "C";
        }
        else  if (avg < 35)
        {
            result = "Fail";
            Grade = "D";
        }
        document.form1.result.value = result;
        document.form1.grade.value = grade;
        document.form1.total.value = total;
        document.form1.average.value = avg;
       
    }
</script>
</head>
<body>
    <form name = "form1">
        <table border = "1">
            <tr>
                <td> Student Name</td>
                <td><input type = "text"  /></td>
            </tr>
            <tr>
                <td colspan = "2" align = "center">Subject Marks</td>
            </tr>
            <tr>
                <td>Web Programming</td>
                <td><input type = "text" name = "wp" /></td>
            </tr>
            <tr>
                <td>Computer Graphics</td>
                <td><input type = "text" name = "cg" /></td>
            </tr>
            <tr>
                <td>System Programming</td>
                <td><input type = "text" name = "sp" /></td>
 
            </tr>
            <tr>
                <td colspan = "2" align = "center"><input type = "button"   onclick = "calc()" value = "calculte" /></td>
            </tr>          
            <tr>
                <td>Total</td>
                <td><input type = "text" name = "total"/></td>
 
            </tr>
            <tr>
                <td>Average</td>
                <td><input type = "text" name = "average" /></td>
            </tr>
            <tr>
                <td>Result</td>
                <td><input type = "text" name = "result" /></td>
            </tr>
            <tr>
                <td>Grade</td>
                <td><input type = "text" name = "grade"/></td>
            </tr>
 
        </table>
    </form>
</body>
</html>
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
9) Develop and demonstrate using jQuery to solve the following:
A) Fade in and fade out all division elements.
B) Animate an element, by changing its height and width.
 
9 Program: -
A) <!DOCTYPE html>
<html>
<head>
<script src="./jquery-1.11.1.min.js"></script>
<title>Fade in and fade out all division elements</title>
</head>
<body>
<div style="background:#2E9AFE;width:100%;">My Effect is fadeIn and fadeOut Effect</div>
<button id="btn2">Fade In (3 Second)</button>
<button id="btn1">Fade Out (3 Second)</button>
 
<script>
$(document).ready(function() {
    $("#btn1").click(function() {
        $("div").fadeOut(3000);
    });
 
    $("#btn2").click(function() {
        $("div").fadeIn(3000);
    });
});
</script>
</body>
</html>
B) <!DOCTYPE html>
<html>
<head>
<script src="./jquery-1.11.1.min.js"></script>
<meta charset="utf-8">
<title>Animate an element, by changing its height and width</title>
</head>
<body>
<button id="btn1">Animate height & width</button>
<button id="btn2">Reset</button>
<div id="box" style="background:#B45F04;height:100px;width:100px;margin:6px;"></div>
<script>
    $( "#btn1" ).click(function() {
  $( "#box" ).animate({
   width: "300px",
   height: "300px",
    }, 1500 );
});
 
$( "#btn2" ).click(function() {
  $( "#box" ).animate({
   width: "100px",
   height: "100px",    
    }, 1500 );
});
 
</script>
</body>
</html>
 
 
 
10) Develop and demonstrate using jQuery to solve the following:
A) Limit character input in the text area including count.  
B) Based on check box, disable/enable the form submit button. 
 
10 Program: -
A) <!DOCTYPE html>
<html>
<head>
<script src="./jquery-1.11.1.min.js"></script>
  <meta charset="utf-8">
  <title>Limit character input in the textarea including count</title>
<style type="text/css">
textarea {
  display:block;
  margin:1em 0;
}  
</style>  
</head>
<body>
<form>
<label>Maximum 15 characters</label>
<textarea id="textarea" maxlength="15"></textarea>
  <span id="rchars">15</span> Character(s) Remaining
</form>
<script>
  var maxLength = 15;
$('textarea').keyup(function() {
  var textlen = maxLength - $(this).val().length;
  $('#rchars').text(textlen);
});
 
</script>
</body>
</html>
 
B) <!DOCTYPE html>
<html>
<head>
<script src="./jquery-1.11.1.min.js"></script>
  <meta charset="utf-8">
  <title>Disable/enable the form submit button</title>
</head>
<body>
<input id="accept" name="accept" type="checkbox" value="y"/>I accept<br>  
<input id="submitbtn" disabled="disabled" name="Submit" type="submit" value="Submit" />
<script>
  $('#accept').click(function() {
  if ($('#submitbtn').is(':disabled')) {
      $('#submitbtn').removeAttr('disabled');
    } else {
      $('#submitbtn').attr('disabled', 'disabled');
    }
});
 
</script>
</body>
</html>
 
