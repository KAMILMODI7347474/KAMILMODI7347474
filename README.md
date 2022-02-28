<!DOCTYPE html>
<head>
  <div class="textbox"><H4>Sign Up/ Log In</H4></div>
  <div class="form"><html>
    <head>
 <title>Form Validation</title>
      <script type="text/javascript">
        var divs = new Array();
        divs[0] = "errFirst";
        divs[1] = "errLast";
        divs[2] = "errEmail";
        divs[3] = "errUid";
        divs[4] = "errPassword";
        divs[5] = "errConfirm";
        function validate()
      {
          var inputs = new Array();
          inputs[0] = document.getElementById('first').value;
          inputs[1] = document.getElementById('last').value;
          inputs[2] = document.getElementById('email').value;
          inputs[3] = document.getElementById('uid').value;
          inputs[4] = document.getElementById('password').value;
          inputs[5] = document.getElementById('confirm').value;
          var errors = new Array();
          errors[0] = "<span style='color:red'>Please enter your first name!</span>";
          errors[1] = "<span style='color:red'>Please enter your last name!</span>";
          errors[2] = "<span style='color:red'>Please enter your email!</span>";
          errors[3] = "<span style='color:red'>Please enter your user id!</span>";
          errors[4] = "<span style='color:red'>Please enter your password!</span>";
          errors[5] = "<span style='color:red'>Please confirm your password!</span>";
          for (i in inputs)
          {
            var errMessage = errors[i];
            var div = divs[i];
            if (inputs[i] == "")
              document.getElementById(div).innerHTML = errMessage;
            else if (i==2)
            {
              var atpos=inputs[i].indexOf("@");
              var dotpos=inputs[i].lastIndexOf(".");
              if (atpos<1 || dotpos<atpos+2 || dotpos+2>=inputs[i].length)
              document.getElementById('errEmail').innerHTML = "<span style='color: red'>Enter a valid email address!</span>";
              else
              document.getElementById(div).innerHTML = "Done!";
            }
            else if (i==5)
            {
              var first = document.getElementById('password').value;
              var second = document.getElementById('confirm').value;
              if (second != first)
              document.getElementById('errConfirm').innerHTML = "<span style='color: red'>Your passwords don't match!</span>";
              else
               document.getElementById(div).innerHTML = "Done!";
            }
            else
              document.getElementById(div).innerHTML = "Done!";
           }
         }
            function finalValidate()
            {
              var count = 0;
              for(i=0;i<6;i++)
              {
                var div = divs[i];
                if(document.getElementById(div).innerHTML == "Done!")
                count = count + 1;
              }
              if(count == 6)
                document.getElementById("errFinal").innerHTML = "Thanks for Sign Up!!!";
            }
       </script>
    </head>
    <body>
      <table id="table1">
          <tr>
            <td>First Name:</td>
            <td><input type="text" id="first" onkeyup="validate();" /></td>
            <td><div id="errFirst"></div></td>
          </tr>
          <tr>
            <td>Last Name:</td>
            <td><input type="text" id="last" onkeyup="validate();"/></td>
            <td><div id="errLast"></div></td>
          </tr>
          <tr>
            <td>Email:</td>
            <td><input type="text" id="email" onkeyup="validate();"/></td>
            <td><div id="errEmail"></div></td>
          </tr>
          <tr>
            <td>User Id:</td>
            <td><input type="text" id="uid" onkeyup="validate();"/></td>
            <td><div id="errUid"></div></td>
          </tr>
          <tr>
            <td>Password:</td>
            <td><input type="password" id="password" onkeyup="validate();"/></td>
            <td><div id="errPassword"></div></td>
          </tr>
          <tr>
            <td>Confirm Password:</td>
            <td><input type="password" id="confirm" onkeyup="validate();"/></td>
            <td><div id="errConfirm"></div></td>
          </tr>
          <tr>
            <td><input type="button" id="create" value="Create" onclick="validate();finalValidate();"/></td>
            <td><div id="errFinal"></div></td>
          </tr>
      </table>
    </body>
    </html></div>
    <HTML>
<HEAD>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Lobster&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="StyleSheet.css">
  <div class="textbox"><H1><i><b><strong>WELCOME TO KAMILS VLOGGING WEBPAGE</strong></b></i></H1></div>
  <div class="logo"><img src="images/KAMILS.png"></div>
  <BODY>
        </BODY>
        </HEAD>
        </HTML>
       <div class="textbox"><h2>My Subscribers in past few months</h2></div>
        <BODY><li>In December I had 5</li>
        <br><li>In January I had 15</li>
        <br><li>In February I have 18</li>
        </BODY>
        </HEAD>
        </HTML>
        <div class="textbox"><h3>Giveaways</h3></div>
        <BODY> I giveaway at
          <br>50 Subscribers
          <br>100 Subscribers
          <br>And whenever I get 50 subscribers + I will Giveaways
          <br>By the way I will giveaway Logos, Intros and Banners means I'll make them for you.
          </BODY>
          </HEAD>
          </HTML>
          
  <p style="font-style:normal;"></p>
  <p style="font-style:italic;">Lets Move <span style="font-style:normal"> </span>On Now.</p>
</body>
</html>
<html>
<head>
<style>
table, th, td {
  border: 1px solid rgb(0, 238, 255);
}
</style>
</head>
<body>

<div class="textbox"><h5>My Identity</h5></div>

<table style="width:100%">
  <tr>
    <th>Firstname</th>
    <th>Lastname</th> 
    <th>Age</th>
  </tr>
  <tr>
    <td>Kamil</td>
    <td>Modi</td>
    <td>12+</td>
  </tr>
  <tr>
    <td>KAMILS</td>
    <td>Vlogging Channel</td>
    <td>2 months 19 days</td>
  </tr>
  <tr>
</table>

</body>
</html>
<html>
<head>
  <title>Page Title</title>
  <link rel="stylesheet" href="mystyle.css">
</head>
<body>

<div class="textbox"><H6>Introducing Kamils Vlogging</H6></div>
<p><br>Wassup, Guys Welcome To My Website KAMILS VLOGGING Please Like Share and Subscribe

  I love Vlogging
  
  I don't use Facebook, Instagram, Snapchat, Twitter and etc
  
  Guys I want you to hep me till 1K subscribers please help me.
         
  <br>~LOVE LOVE 💖💖💖
  
  <br><br>TO VIEW MY Website CLIK HERE =
  <nav>
    <ul>
      <a href="https://www.youtube.com/channel/UCYsTx_KABPLXPBiMrr2eqcw?sub_confirmation=1">CLICK HERE</a>
</body>
</html>
    <div class="textbox"></div><h6>Old channel Vs New channel</h6></div>
    <html>
<head>
<title>Old VS New</title>
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
</head>
<body>

<div class="w3-container w3-aqua">
  <h1>Old Channel Vs New Channel</h1> 
  <p>Scroll Down!😁</p> 
</div>

<div class="w3-row-padding">
  <div class="w3-third">
    <h2>Kamil Modi</h2>
    <p>It took me almost 5 months to gain 30 subscribers and 2 years for 116 Subscribers.
      <br>I made logo so many times and intros also, but they were not so good.
    </p>
  </div>

  <div class="w3-third">
    <h2>Kamils Vlogging</h2>
    <p>It took me only 3 and half months to gain 18 subscribers.</p> 
    <p>Now please help me to gain 1K subscribers.
      <br> I designed the logo and made the intro once and awesome.
    </p>
  </div>
</body>
</html>
<div class="textbox"><br><br><br><br><br><br><br><br><br><br><H8>My banner</H8></div>
<div class="bannernew"><img src="images/Banner New.png"></div>
<div class="newtext"><h11>MY SHORT BIOGRAPHY</h11></div>
<html>
<style>
table, th, td {
  border:1px solid rgb(0, 225, 255);
}
</style>
<body>
<table style="width:100%">
  <tr>
    <th>Name</th>
    <th>Age</th>
    <th>Nationality</th>
    <th>Hobby</th>
    <th>Favorite Movie</th>
    <th>Favortie fast food</th>
    <th>Favorite food</th>
    <th>Profession</th>
  </tr>
  <tr>
    <td>Kamil Modi</td>
    <td>12+</td>
    <td>Indian</td>
    <td>Vlogging</td>
    <td>Uncharted</td>
    <td>Pizza</td>
    <td>Biryani</td>
    <td>Designing</td>
  </tr>
  </tr>
</table>
</body>
</html>
<div class="textbox"><H13>My one of the longest video<H13></div>
  <html>
<body>

<div class="center"><iframe width="600" height="600" src="https://www.youtube.com/embed/zACmwphbWeQ"></iframe></div>
</iframe>
</body>
</html>
