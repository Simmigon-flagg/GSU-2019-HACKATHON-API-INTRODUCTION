# GSU-2019-HACKATHON-API-INTRODUCTION

Mac Users open 
Terminal 

PC Users open
Commandline

Type or copy paste  curl -I http://www.google.com to view the header.

Type or copy paste  curl  http://www.google.com to view the data return.

For some of these Demo you will need a GitHub account.

Github API

Go to https://github.com/  and sign up for an account like you would do any other sign up.

To Follow me on GitHub click here  https://github.com/simmigon-flagg and I’ll follow you back. You can see all of my publish repos and what I post in the future.

Type or copy paste  curl -I  https://api.github.com/ to view the data return.

Type or copy paste  curl  https://api.github.com/users/{user} to view the data return.

To learn more about the GitHub api copy or paste https://developer.github.com/v3/ into an URL search bar.

POSTMAN

A User Interface for Testing API. https://www.getpostman.com/downloads/

Dark Sky API

Go to https://darksky.net/dev and sign up for an account like you would do any other sign up.

Dark Sky and POSTMAN

Webpages, APIs and Browser Developer tool

To developer code I use https://code.visualstudio.com/ Feel free to use any code editor you like but it will be easier to follow alone with these Demos

View in console 

 https://jsonplaceholder.typicode.com/

1 . Copy
    <!--Import Google Icon Font-->
    <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet"
    />

    <!-- Compiled and minified CSS -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0/css/materialize.min.css"/>

    <!-- Compiled and minified JavaScript -->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>

    <!--Let browser know website is optimized for mobile-->
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" type="text/css" href="main.css" />


1.  Copy
	//import my-api.js into the project
    <script type="text/javascript" src=“my-api.js"></script>

1.  Copy
	// The main users Profile
        <div class="w3-card w3-round w3-white">
          <div class="w3-container">
           <h4 id=username class="w3-center" >My Profile</h4>
           <div id="photo"></div>


           <hr>
           <p><i class="fa fa-pencil fa-fw w3-margin-right w3-text-theme"></i> Designer, UI</p>
           <p><i class="fa fa-home fa-fw w3-margin-right w3-text-theme"></i><span id="userlocation" ></span></p>
           <p><i class="fa fa-birthday-cake fa-fw w3-margin-right w3-text-theme"></i><span id="userbirthday" ></span></p>
          </div>
        </div>

1.  Copy
	//The post from friends
        <div class="w3-container w3-card w3-white w3-round w3-margin"><br>
          <div id="photo1"></div>

          <span class="w3-right w3-opacity">1 min</span>
          <h4 id="username1">John Doe</h4><br>
          <hr class="w3-clear">
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
            <div class="w3-row-padding" style="margin:0 -16px">
  
          </div>
          <button type="button" class="w3-button w3-theme-d1 w3-margin-bottom"><i class="fa fa-thumbs-up"></i>  Like</button> 
          <button type="button" class="w3-button w3-theme-d2 w3-margin-bottom"><i class="fa fa-comment"></i>  Comment</button> 
        </div>
        
        <div class="w3-container w3-card w3-white w3-round w3-margin"><br>
          <div id="photo2"></div>
      
          <span class="w3-right w3-opacity">16 min</span>
          <h4 id="username2" >Jane Doe</h4><br>
          <hr class="w3-clear">
          <p>Lorem ipsum dolor sitå amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
          <button type="button" class="w3-button w3-theme-d1 w3-margin-bottom"><i class="fa fa-thumbs-up"></i>  Like</button> 
          <button type="button" class="w3-button w3-theme-d2 w3-margin-bottom"><i class="fa fa-comment"></i>  Comment</button> 
        </div>  
  
        <div class="w3-container w3-card w3-white w3-round w3-margin"><br>

          <div id="photo3"></div>

          <span class="w3-right w3-opacity">32 min</span>
          <h4 id="username3">Angie Jane</h4><br>
          <hr class="w3-clear">
          <p>Have you seen this?</p>
          <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
          <button type="button" class="w3-button w3-theme-d1 w3-margin-bottom"><i class="fa fa-thumbs-up"></i>  Like</button> 
          <button type="button" class="w3-button w3-theme-d2 w3-margin-bottom"><i class="fa fa-comment"></i>  Comment</button> 
        </div> 

1.  Copy
        <div class="w3-card w3-round w3-white w3-center">
            <div class="w3-container">
              <p>Weather Dark Sky</p>
              <!-- <img src="/w3images/forest.jpg" alt="Forest" style="width:100%;"> -->
  
              <p id="currently-summary"></p>
              <p id="currently-time" >Friday 15:00</p>
              <p><button class="w3-button w3-block w3-theme-l4">Info</button></p>
            </div>
          </div>


Inside of 

1.  Copy
 Var my_URL;
$.ajax({
  url: my_URL,
  dataType: 'json',
  method:'GET',
  success: function(data) {
// Paste 2
// Paste 3
// Paste 4
// Paste 5
// Paste 6

},
  error: function(data) {
// Paste 7
}
});

2.copy
    //User to get son data
    alert(JSON.stringify(data));
    alert(Object.keys(data));
    alert(Object.values(data));
    console.log(data.results[0]);
	/*
	for(n in data){
	console.log(data[n]);
}
*/

3.$(“#userlocation").html(data.results[0].location.city.toUpperCase() + ", " +data.results[0].location.state.toUpperCase());
4 $("#userbirthday").html(data.results[0].dob.date.split("T")[0]); 
5 $("#username").text(data.results[0].name.first.toUpperCase() + " " + data.results[0].name.last.toUpperCase());  
6 $("#photo").html('<p class="w3-center"><img src="'+data.results[0].picture.large+'" class="w3-circle" style="height:106px;width:106px" alt="Avatar"></p>'); 
7 alert("User Data Did not load!");

8.
    var lo = data.results[0].location.coordinates.longitude;
    var la = data.results[0].location.coordinates.latitude;
    getWeather(lo,la);

9.
//function getWeather(long, lat){

  var myURL = "https://api.darksky.net/forecast/85dcf97c6c19448d76fb2ee8a80fd322/"+long+"," + lat;
  // var queryURL = "https://api.github.com/users/Simmigon";
  
  $.ajax({
    url: myURL,
    dataType: 'jsonp',
    success: function(data) {
      // console.log(JSON.stringify(data));
      // console.log(Object.keys(data));
      // console.log(Object.values(data));
      console.log(data);
      console.log(data.currently.summary);
      $("#currently-summary").text("Current: " + data.currently.summary.toUpperCase()); 
      $("#currently-time").text("Time: " + data.currently.time); 

    },
    error: function(XMLHttpRequest, textStatus, errorThrown) {
      alert("Forcast Did not load!");
   }
  });

}









