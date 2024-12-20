# Ex.05 Design a Website for Server Side Processing
## Date:08/12/2024

## AIM:
 To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side. 


## FORMULA:
P = I<sup>2</sup>R
<br> P --> Power (in watts)
<br> I --> Intensity
<br> R --> Resistance

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<html>
    <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>Math Server</title>
        <style>
         div {
              margin-top: 12%;
         }
         form {
              width: 450px;
              height: 200;
              border: 2px solid black;
              padding: 50px;
              line-height: 10px;
              font-size: 32px;
              background: rgb(34, 33, 34);
         }
         body{
              background-image: url("/static/energy.jpg");
              background-repeat: no-repeat;
              background-attachment: fixed;
              background-size: cover;
         }
         h1{
              color: #15b1f9;
              font-size: 40px;
              margin-top: 0;
              margin-bottom: 10%;
         }
         input{
              border-radius: 15px;
              margin-left: 10px;
              font-size: 32px;
         }
         .i{
               cursor: pointer;
               box-sizing: border-box;
               background-color: #b863f8;
               padding-left: 100px;
               padding-right: 100px;
         }
         label{
               color: #a00707;
               font-size: 40px;
               margin-bottom: 10%;
         }
        </style>
        <script>
                function calc(){
                  var a=Number(document.getElementById("t1").value);
                  var b=Number(document.getElementById("t2").value);
                  document.getElementById('t3').innerText ="Power: "+a*a*b +'W';
                }
        </script>
    </head>
    <body>
        <div>
            <center>
               <form>
                   <h1>Power Calculator</h1>
                   <input type="text" name="Current" id="t1" placeholder="Enter Intensity" ><br><br>
                   <input type="text" name="Resistance" id="t2" placeholder="Enter Resistance" ><br><br>
                   <input type="button" value="Calculate" onclick="calc();" class="i" ><br><br><br>
                   <label id="t3"></label>
                </form>
            </center>
        </div>
    </body>
</html>  
```

## SERVER SIDE PROCESSING:
```
        <script>
                function calc(){
                  var a=Number(document.getElementById("t1").value);
                  var b=Number(document.getElementById("t2").value);
                  document.getElementById('t3').innerText ="Power: "+a*a*b +'W';
                }
        </script>
```

## HOMEPAGE:

![alt text](math.png)

## RESULT:
The program for performing server side processing is completed successfully.
