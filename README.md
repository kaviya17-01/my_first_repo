
/* Add code for container class below */
.container {
    /* Add rules here */
    diaplay:grid;
    max-width: 900px;
    min-height: 50vh;
    grid-template-columns: 100%;
    grid-template-rows: auto auto 1fr auto auto;
    grid-template-areas: "header" "left" "main" "right" "footer";
}
/* Add media rules for container class below */
@media (min-width: 440px) {
    .container {
    /* Add rules here */
    grid-template-columns: 150px 1fr 150px;
    grid-template-rows: auto 1fr auto;
    grid-template-areas: "header header header" 
                         "left main right" 
					               "footer footer footer";
    }
}


/* Properties for other selectors */
.header {
    grid-area: header;
    padding: 10px;
    background-color:black;
    color: #fff;
    text-align: center;
}
  
.main {
    grid-area: main;
    padding: 25px;
}
  
.left {
    grid-area: left;
    background-color: peachpuff;
  }
  
.right {
    grid-area: right;
  }
  
.footer {
    grid-area: footer;
    padding: 10px;
    background-color:black;
    color: #fff;
    text-align: center;
  }
  
.sidebar {
    padding: 25px;
    background-color:darkcyan;
  }

HTML
<!DOCTYPE html>

<html>
<head>
  <link rel="stylesheet" href="style.css">
</head>

<body>
    <div class="container">
        <header class="header"> Header </header>
        <main class="main"> Content </main>
        <div class="sidebar left"> Sidebar </div>
        <div class="sidebar right"> Sidebar </div>
        <footer class="footer"> Footer </footer>
    </div>
</body>

</html>
