# In Name Of God!

# Code:

     <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>
    <body style="font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;">
        <div  id="stting" style="background-color: white; border: none; margin-left: 110px; width: 1100px; height: 750px; border-radius: 10px; box-shadow: 2px 2px 10px; margin-top: 40px;">
            <br>
            <h1 style="text-align: center; font-size: 40px;">Setting > Costome</legend>
            <br><br>
            <textarea type="text" id="text" style="text-align: center; font-size: 30px; height: 100px;" placeholder="Your Text Web Log"></textarea>
            <br><br>
            <input type="text" id="titel" placeholder="Titel Web Log" style="border-radius: 5px; height: 40px; font-size: 20px;">
            <br><br>
            <input type="text" id="color" placeholder="Code Color To background" style="border-radius: 5px; height: 40px; font-size: 20px;">
            <br><br>
            <button class="b" id="hi" style="background-color: rgb(112, 112, 192);"id="h">height</button>
            <button class="b" id="im" style="background-color: rgb(112, 112, 192);" id="new-img">New Img</button>
            <br><br>
            <button id="save" class="b">Save</button>
        </div>

        <div id="log" style="background-color: white; border: none; margin-left: 110px; width: 1100px; height: 500px; border-radius: 10px; box-shadow: 2px 2px 10px; margin-top: 40px;">
            <br>
            <h1 id="t2" style="text-align: center; font-size: 40px;">Your Web log!</legend>
            <br><br>
            <h2 id="t" style="color: brown; text-align: center; font-size: 40px;">(None)</h2>
            <br><br>
            <button id="start" class="b">Start</button>
            </div>

        <style>
            .b {
                background-color: rgb(53, 145, 53);
                text-align: center;
                color: white;
                width: 150px;
                height: 50px;
                font-size: 30px;
                margin-left: 470px;
                border-radius: 8px;
                border: none;
                transition: 1s;

            }
            .b:hover {
                box-shadow: 1px 1px 10px black;
            }
        </style>

        <script>
            document.getElementById("stting").style.display = "none"
            alert("Welcom")
            // =======================================
            document.getElementById("start").addEventListener("click", function(){
                document.getElementById("stting").style.display = ""
                document.getElementById("log").style.display = "none"  
            })
            document.getElementById("hi").addEventListener("click", function(){
                    var hi = prompt("Your height: ")+"px"
                    document.getElementById("log").style.height = hi
                }) 
            document.getElementById("im").addEventListener("click", function(){
                var src2 = prompt("Your Addres Img: ")
                var img = document.createElement("img")
                img.src = src2
                img.id = "i3"
                document.getElementById("log").appendChild(img)
                document.getElementById("i3").style.marginLeft = "330px"
                document.getElementById("i3").style.borderRadius = "10px"
            })
            document.getElementById("save").addEventListener("click", function(){
                document.getElementById("t2").style.color = "brown"
                document.getElementById("t").style.color = "black"
                document.getElementById("t").innerHTML = document.getElementById("text").value
                document.getElementById("t2").innerHTML = document.getElementById("titel").value
                document.body.style.backgroundColor = document.getElementById("color").value
                document.getElementById("stting").style.display = "none"
                document.getElementById("log").style.display = "" 
                document.getElementById("start").style.display = "none"
            })
        </script>
    </body>
    </html>
    
   
# Program:
Html, Css, Js

