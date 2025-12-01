<!DOCTYPE html>
<html>
    <head>
        <script>
            function keyup()
            {
                document.getElementById("key-status").innerHTML="key up";
            }
            function keydown()
            {
                document.getElementById("key-status").innerHTML="key down";
            }
            function keypress(event)
            {
                document.getElementById("key-status").innerHTML="key press:"+ event.key;
            }
        </script>
    </head>
        <body>
            <h2>Keyboard Event in JavaScript</h2>
            <input type="text" placeholder="press anykey" 
            onkeyup="keyup()"
            onkeydown="keydown()"
            onkeypress="keypress(event)">
            <p id="key-status" style="color:blue;font-size: 20px;font-family: Arial, Helvetica, sans-serif"></p>
            <p id="key-press" style="color:green;font-size: 20px;font-family: Arial, Helvetica, sans-serif"></p>
        </body>
</html>
