<!DOCTYPE html>
<html>
    <head>
        <style>
            #box {
                width: 200px;
                height: 200px;
                background-color: lightblue;
                border: 2px solid black;
            }   
        </style>
        <script>
            function box1() {
                document.getElementById("box").style.color = "red";
                document.getElementById("box").style.backgroundColor = "lightgreen";
            }
            function box2() {
                document.getElementById("box").style.color = "black";
                document.getElementById("box").style.backgroundColor = "lightblue";
            }
            function display() {
                document.getElementById("btn").innerHTML = "double clicked";
            }
        </script>
    </head>
    <body>
        <div id="box" onmouseover="box1()">
            <p>BOX</p>
        </div>
        <div id="box" onmouseout="box2()">
            <p>BOX</p>
        </div>
        <button id="btn" ondblclick="display()">click me</button>
    </body>
</html>
