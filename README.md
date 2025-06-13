<!DOCTYPE html>
<html>

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  
  <link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono&display=swap" rel="stylesheet">
  <title></title>
  <style>
    body{
      font-family: 'Fira Code', monospace;
      display: flex;
      justify-content: center;
      align-items: center;
    }
   h1{
     font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
     font-weight: bold;
     font-family: 'JetBrains Mono', monospace;
     font-size: 20px;
     font-family: Georgia, 'Times New Roman', Times, serif;
   }
   p{
     font-size: 15px;
   }
   .id{
  text-align: center;
     align-items: center;
   }
   #select{
     padding: 17px;
     border: none;
     display: flex;
     flex-direction: column;
     border-radius: 20px;
     align-items: center;
     justify-content: center;
   }
   body.dark{
     background: #000000;
     color: white;
   }
   body.light{
     font-family: 'Fira Code', monospace;
   }
  </style>
</head>

<body>
  <div class="id">
      <h1 id="h1"> Hello, check it out</h1>
  <p>pick your style</p>
  <select name="" id="select"
  >
    <option value="light">
      🔥 light mode
    </option>
    <option value="dark">
      🌜 dark mode
    </option>
  </select>
  </div>

</body>
<script>

let h1 = document.getElementById("h1")
 let pr = prompt("Add username")
 console.log(pr)
h1.textContent = `Hello,${pr} choose`
  let theme = document.getElementById("select")
  theme.addEventListener(
    "change", 
    //document.body.classList.remove("light", "dark", "style");
    
    function(){
      document.body.classList = this.value 
    }
   
  )
</script>


</html>
