<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body class="m1">
   <div class="user">
        <div class="main">
            <form onsubmit="return data()"  action="abc.html">
                 UserId:<input type="text" id="n1"> 
                 Contact:<input type="text" id="n2"> 
                 password:<input type="password" id="n3"> 
                 confirm password:<input type="password" id="n4"> 
                 <input type="submit" value="submit you data">
            </form>
        </div>
   </div>
</div>
</body>
<script>function data(){
    var a=document.getElementById("n1").value;
    var b=document.getElementById("n2").value;
    var c=document.getElementById("n3").value;
    var d=document.getElementById("n4").value; 

    if( a=="" || b=="" || c=="" || d=="" ){ 
        alert("all fields are mendatory!");
        return false;
    }
    else if(b.length<10 || b.length>10){ 
        alert(" please Enter 10 digit numer");
        return false;
    }
    else if(isNaN(b)){ 
        alert("only number are allowed ");
     return false;
    }
    else if(c!=d){ 
        alert("not passwerd same !");
     return false;
    }
    else{
        true;
    }
}
</script>
</html>
