<!DOCTYPE html>
<html>
    <head>
    <title>Form Validation</title>
    <script>
        function validform(){
            let name=document.myform.username.value;
            let email=document.myform.email.value;
            if(name==""){
                alert("please enter your name");
                return false;
            }
            if(email==""){
                alert("Please enter your email");
                return false;
            }
            let pattern=/^[^ ]+@[^ ]+\.[a-z]{2,3}$/;
            if(!email.match(pattern)){
                alert("Please enter a valid email address");
                return false;
            }
            alert("Form submitted successfully");
            return true;
        }
    </script>
    </head>
    <body>
        <form name="myform" onsubmit="return alidform()">
            Name  <input type="text" id="name" name="name"><br><br>
            Email <input type="email" id="email" name="email"><br><br>
            <input type="submit" value="Submit">
        </form>
    </body>
</html>
