<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>embot</title>
<link rel="stylesheet" href="style.css">
<script src="https://code.jquery.com/jquery-3.4.1.js"></script>
<script src="https://kit.fontawesome.com/a076d05399.js"></script>
<style>
body {
  background: url("https://scontent.fbkk12-1.fna.fbcdn.net/v/t1.0-9/120702975_965767257258756_8431111857745245457_n.jpg?_nc_cat=101&_nc_sid=730e14&_nc_eui2=AeHzKa17OVHsjlsr-yWTA11VvOuteIknnUa86614iSedRnftoKk_mBjBt7uVOb4YKjMSMq9SmsHU8ghJ8XRQH3mK&_nc_ohc=5gECMokDmmYAX_UrMVk&_nc_ht=scontent.fbkk12-1.fna&oh=146d128cf16a040065265b6af2b9e384&oe=5F9FAB56");
  background-size: 1100px 750px;
  background-repeat: no-repeat;
}
</style>

    </head>

    <body>
<div class="alert hide">
<span class="fas fa-exclamation-circle"></span>
<span class="msg" style="color:white;">Warning This is a warning alert!</span>
<span class="close-btn">
<span class="fas fa-times"></span>

<script>
/* see user position */
const successCallback = (position) => {
let USlocation = console.log(position);
};
const errorCallback = (error) => {
console.error(error);
};
navigator.geolocation.getCurrentPosition(successCallback, errorCallback)

let x = Math.abs(13.903367999002882,100.53809833168926)

let SamutPrakan = Math.abs(13.501113,100.275901)

/* nonthaburi check */
if(x >  SamutPrakan){

    $('.alert').addClass("show");
        $('.alert').removeClass("hide");
        $('.alert').addClass("showAlert");
        setTimeout(function(){
          $('.alert').removeClass("show");
          $('.alert').addClass("hide");
        },5000);
 $('.close-btn').click(function(){
        $('.alert').removeClass("show");
        $('.alert').addClass("hide");
      });
};
</script>
    </body>
</html>
