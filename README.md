<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body {
  font-family:Helvetica;
}

.flip-card {
  background-color: #ffffff;
  width: 528px;
  height: 305px;
  perspective: 1000px;
}

.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.6s;
  transform-style: preserve-3d;
  box-shadow: 8px 4px 8px 8px rgba(0,0,0,0.2);
}

.flip-card:hover .flip-card-inner {
  transform: rotateY(180deg);
}

.flip-card-front, .flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
}

.flip-card-front {
  background-color: #ffffff;
  color: black;
}

.flip-card-back {
  background-color: #ffffff;
  color: black;
  transform: rotateY(180deg);
}
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  padding: 5px;
  text-align: left;
}
.button {
  background-color: #e7e7e7; /* Green */
  border: none;
  color: black;
  padding: 10px 21px;
  text-align: center;
  text-decoration: bold;
  display: inline-block;
  font-size: 17px;
  margin: 4px 2px;
  cursor: pointer;
}
</style>
</head>
<body>

<div class="flip-card">
  <div class="flip-card-inner">
    <div class="flip-card-front">
      <img src="https://raw.githubusercontent.com/breatheco-de/exercise-postcard/main/.learn/assets/4geeks.png" alt="Avatar" style="width:300px;height:300px;">
    </div>
    <div class="flip-card-back">
     <table>
  <tr><td> 
      <h1 style="text-align:left;padding:5px">MY POSTCARD</h1>
       <p style="text-align:left;padding:5px"><i><b>Look how awesome! This is a postcard that I created using HTML5 and CSS3 during my 4Geeks Academy Course!<br><br>This is so cool, can't wait to start doing more stuff!</b></i></p></td>
  <td><img alt="Avatar" style="float:right; width:auto;height:90px;padding:5px" src="https://raw.githubusercontent.com/breatheco-de/exercise-postcard/main/.learn/assets/4geeks.png" ><form style="text-align:right;padding:5px">
  
  <input type="Name" id="Name" value="Some Name"><br><br>
  <input type="email" id="Email" value="Some Email"><br><br>
  <input type="text" id="lname" value="Some comment">
</form></td>
  </tr>
</table>
<button class="button" onclick="alert('Hello world!')"><b>SEND MY POSTCARD</b></button>
 </div>

   
    
    </div>
  </div>
</div>

</body>
</html>
