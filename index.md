<html>
<body>
<center>
<input type="text" placeholder="&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Iyong pangalan" id="name">
<br>
</br>
<input type="button" value="Pindut" onClick="testing();">
</center>
<style type="text/css">
center {
  margin-top: 300px;
}
input[type="button"] {
  color: rgb(0,64,255);
  background-color: white;
  border-color: rgb(0,64,255);
  font-size: 17px;
  border-radius: 25px;
  padding: 3px;
}
input[type="text"] {
  background-color: white;
  border-top: none;
  border-left: none;
  border-right: none;
  border-color: rgb(0,64,255);
  font-size: 20px;
  border-radius: 25px;
  padding:3px;
}
</style>
<script type="text/javascript">
function testing() {
  var nam = document.getElementById("name").value;
  if (nam.length >= 1) {
    var num = Math.floor(Math.random() * 100) + 1;
    alert(nam + " Is " + num + "% Handsome\n" + checks(num));
  } else {
    alert("Bawal ang blangko be!");
  }
}
function checks(num) {
  if (num >= 40 && num <= 60) {
    return "Satingin ko ikaw ay normal.";
  }
  else if (num <= 40 && num >= 0) {
    return "Pasensya be ikaw ay panget!";
  }
  else if (num >= 60 && num <= 100) {
    return "Napaka CUTE mo!";
  }
  else {
    return "HMMMM...";
  }
}
</script>
</body>
</html>
