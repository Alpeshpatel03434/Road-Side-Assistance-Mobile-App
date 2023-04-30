# Road-Side-Assistance-Mobile-App

<div style="">
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
/* Style the buttons */
.btn {
  border: none;
  outline: none;
  padding: 10px 16px;
  background-color: #f1f1f1;
  cursor: pointer;
  font-size: 18px;
}

/* Style the active class, and buttons on mouse-over */
.active, .btn:hover {
  background-color: #666;
  color: white;
}
</style>
</head>
<body>

<h1>Active Button</h1>
<p>Highlight the active/current (pressed) button.</p>
  
<div id="myDIV">
  <button value="1" class="btn active">1</button>
  <button value="2" class="btn">2</button>
  <button id="3" value="3" class="btn">3</button>
  <button value="4" class="btn">4</button>
  <button value="5" class="btn">5</button>
</div>

<script>

var container = document.getElementById('myDIV');
container.addEventListener("click", showNumber)
function showNumber(event) {
  const clickedThing = event.target;
  if(clickedThing.tagName == 'BUTTON'){ // makes sure this click interests us
    alert(clickedThing.value);
  }
}

var btns = container.getElementsByClassName("btn");

for (var i = 0; i < btns.length; i++) {
  btns[i].addEventListener("click", function() {
  var current = document.getElementsByClassName("active");
  current[0].className = current[0].className.replace(" active", "");
  this.className += " active";
  });
}

</script>

</body>
</html>

</div>

Road Side Assistance is the application that will help person to find any service provider if their vehicle is immobilized due to an accident or electrical/ mechanical failure, the vehicle is towed free to nearest garage up to few kilometers. This application uses live GPS Tracking for both the users to get live updates. Registered partners will be notified and will accept the request. The Road Side Assistance will be developed with the aim of providing emergency road side assistance services round the clock to ensure a pleasurable and uninterrupted journey virtually anywhere.

Location based vehicle service is the web application that will help person to find any service provider if their vehicle is immobilized due to an accident or electrical/ mechanical failure, the vehicle is towed free to nearest garage up too few kilometres. The Location based vehicle service application will be developed with the aim of providing emergency road side assistance services round the clock to ensure a pleasurable and uninterrupted journey virtually anywhere.


### App Screenshot <a href="https://github.com/Alpeshpatel03434/Road-Side-Assistance-Mobile-App/blob/master/App%20Screenshot.pdf">View (Click)</a> here
