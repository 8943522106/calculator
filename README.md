<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="">
    <title>Calculator</title>
    
</head>
<body>
<div class="container">
    <div class="calculator">
        <input type="text" placeholder="0" id="output-screen">
        <button onclick="Clear()">Cl</button>
        <button onclick="del()">DEL</button>
        <button onclick="display('%')">%</button>
        <button onclick="display('/')">/</button>
        <button onclick="display('7')">7</button>
        <button onclick="display('8')">8</button>
        <button onclick="display('9')">9</button>
        <button onclick="display('*')">*</button>
        <button onclick="display('4')">4</button>
        <button onclick="display('5')">5</button>
        <button onclick="display('6')">6</button>
        <button onclick="display('-')">-</button>
        <button onclick="display('1')">1</button>
        <button onclick="display('2')">2</button>
        <button onclick="display('3')">3</button>
        <button onclick="display('+')">+</button>
        <button onclick="display('.')">.</button>
        <button onclick="display('0')">0</button>
        <button  onclick="display()">=</button>
        
       
    </div>
</div>
<script> 
let outputScreen = document.getElementById("output-screen");

function display(num){
    outputScreen.value += num;
}
function Calculate(){
    try{
        outputScreen.value = eval(outputScreen.value);
    }
    catch(err)
    {
        alert("Invalid")
    }
}
</script>

    
</body>
</html>
