<html>
     <head>
          <meta charset = "utf-8">
          <style>

          </style>
     </head>
     <body>
          <h1>Testing JS</h1>
          <button id="button">Button</button>
          <script>
               var count = 0;
               var button = document.getElementById("button");
               var onClick = function() {
                    count++;
                    button.textContent = "Clicked " + count + " time" + (count>0 ? "s" : "");
                    if (count>=5 & count<10) button.setAttribute("style","background-color: red;");
                    else if (count>=10) button.setAttribute("style","background-color: blue;");
               }
               button.addEventListener("click",onClick);
          </script>
     </body>
</html>
