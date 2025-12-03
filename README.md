<!DOCTYPE html>
<html>
    <head>
        <title>Mouse Events</title>
        <script>
            function singleClick() {
                document.getElementById("mouse-msg").innerHTML = "Single Click Event Triggered";
            }
            function doubleClick() {
                document.getElementById("mouse-msg").innerHTML = "Double Click Event Triggered";
            }
            function mouseOver() {
                document.getElementById("mouse-msg").innerHTML = "Mouse Over Event Triggered";
            }
            function mouseOut() {
                document.getElementById("mouse-msg").innerHTML = "Mouse Out Event Triggered";
            }
            function mouseMove() {
                document.getElementById("mouse-msg").innerHTML = "Mouse Down Event Triggered";
            }
        </script>
    </head>
    <body>
        <h2>Mouse based Event</h2>

        <div style="width:300px; height:150px;background:rgb(255, 128, 0); border: 2px solid black;"
            onclick="singleClick()"
            ondblclick="doubleClick()"
            onmouseover="mouseOver()"
            onmouseout="mouseOut()"
            onmousedown="mouseMove()">
            <p> move/ Click Inside This Box</p>
        </div>
        <p id="mouse-msg" style="color:blue;font-weight:bold;"></p>
    </body>
</html>
