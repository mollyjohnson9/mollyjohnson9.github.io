<!DOCTYPE html>
<html>
<body>

<div class="tab">
  <button class="tablinks" onclick="openCity(event, 'Home')"id="defaultOpen">Home</button>
  <button class="tablinks" onclick="openCity(event, 'Lacrosse')">Lacrosse</button>	
</div>
<script>
// Get the element with id="defaultOpen" and click on it
document.getElementById("defaultOpen").click();
</script>

<div id="Home" class="tabcontent">
	<h1 style="text-align:center; background-color:maroon; color:white;font-size:60px;">
	Molly Saylor Johnson
	<br>
	Fightin' Texas Aggie Class of '22!
	</h1>

<hr>
<center>
<img src="gig em.jpg" width="350px" height="500px">
<img src="orderedring.jpg" width="350px" height="500px">
<img src="treepic.jpg" width="350px" height="500px">
</center>
<hr>

<p style="background-color:lightgrey;font-size:30px;">
<b style="font-size:40px;">Welcome to my portfolio!</b>
<br>
The purpose of this website is to reflect upon important moments from my
years as a college student. Each year I update the pages to talk about what has changed 
and how I've grown. This website has in fact been coded by myself in HTML! 
</p>
</div>

<div id="Lacrosse" class="tabcontent">
  <h1 style="text-align:center; background-color:maroon; color:white;font-size:60px;">
  TAMU Women's Lacrosse Team</h1>
<center>
  <hr>
  <img src="beachteampic.jpg" width="1000px" height="600px">
<hr>
</center>

  <p style="font-size:20px;">
<b style="font-size:30px;"> Year 1: Meeting a New Team</b><br>
I have played lacrosse for over 10 years now, so I knew even before coming to A&M that I wanted to play for their club team.
Lacrosse has always been important to me because the sport taught me a lot about responsibility and time management.
(It was also a great way to keep the freshman 15 away.) 

</p>
</div>

<script>
function openCity(evt, cityName) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablinks");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].className = tablinks[i].className.replace(" active", "");
  }
  document.getElementById(cityName).style.display = "block";
  evt.currentTarget.className += " active";
}
</script>

</body>
</html>
