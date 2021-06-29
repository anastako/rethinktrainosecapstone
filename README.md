<!DOCTYPE html>
<html lang="en">
<head>
<title>Page Title</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body {
  font-family: Arial, Helvetica, sans-serif;
}
</style>
</head>
<body>

<h1>Konstantinos Anastasiou</h1>
<p>Rethink TrainOse prototype.</p>
<div id="main">
  <div id="iphone-x">
    <div id="speaker"></div>
    <div id="camera"></div>
    <iframe width="375" height="812" src="https://xd.adobe.com/embed/5700bc3d-d0f9-4280-572f-da43c58103d7-2131/screen/3db3a46e-4de0-43bd-ab98-fcb7b4e1cfe2?fullscreen" frameborder="0" allowfullscreen></iframe>
  </div>  
</div>
<style>
body { 
  background-image: none;
  background-size: cover;
  background-position: center;
}
 
#main {
  min-height: 100vh; 
  display: flex;
  justify-content: center;
  align-items: center;
}

#iphone-x {
  position: relative;
  margin: 40px auto;
  width: 375px;
  height: 812px;
  border-radius: 40px;
  background-color: #1f1f1f;
  box-shadow: 0px 0px 0px 11px #1f1f1f, 0px 0px 0px 13px #191919, 0px 0px 0px 20px #111, 8px 8px 40px #000;
  overflow: hidden;
  
  &:before,
  &:after{
    content: '';
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
  }
  
  // home button indicator
  &:after {
    bottom: 7px;
    width: 140px;
    height: 4px;
    background-color: #f2f2f2;
    border-radius: 10px;
  }
  
  // frontal camera/speaker frame
  &:before {
    top: 0px;
    width: 56%;
    height: 30px;
    background-color: #1f1f1f;
    border-radius: 0px 0px 40px 40px;
  }
  
  // speaker
  #speaker {
    position: absolute; 
    top: 0px;
    left: 50%;
    z-index: 2;
    transform: translate(-50%, 6px);
    height: 8px;
    width: 15%;
    background-color: #101010;
    border-radius: 8px;
    box-shadow: inset 0px -3px 3px 0px rgba(256, 256, 256, 0.2);
  }
  
  // camera
  #camera {
    position: absolute;
    left: 10%;
    top: 0px;
    z-index: 3;
    transform: translate(180px, 4px);
    width: 12px;
    height: 12px;
    background-color: #101010;
    border-radius: 12px;
    box-shadow: inset 0px -3px 2px 0px rgba(256, 256, 256, 0.2);
    
    &:after {
      content: '';
      position: absolute;
      background-color: #2d4d76;
      width: 6px;
      height: 6px;
      top: 2px;
      left: 2px;
      top: 3px;
      left: 3px;
      display: block;
      border-radius: 4px;
      box-shadow: inset 0px -2px 2px rgba(0, 0, 0, 0.5);
    }
  }
  
}
</style>
</body>
</html>
