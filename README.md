# DiceRoll
Simple browser based program to roll dice and generate random numbers between 1-6 every 5 seconds

<!DOCTYPE html>
<html>
<head>

#Set a bigger font size by modifying <em> HTML tag 
<style>
em {
  font-size: 550px;
}
</style>

</head>
<body>
<center>

<h2>My Dice Roller</h2>

#Call JavaScript element "dice" defined in the JavaScript function diceroll() defined below 
<em id="dice"></em>


<script>

#Define JavaScript function to generate random number between 1 and 6
function diceroll() {
document.getElementById("dice").innerHTML =
Math.floor(Math.random() * 6) + 1;
}

#Use setInterval to call the direroll() function every 5 seconds
setInterval(diceroll, 5000);
</script>

</center>
</body>
</html>
