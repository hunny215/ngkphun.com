<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8" name="viewport" content="width=device-width, initial-scale = 1">
    <title>For ngkphun</title>
    <style>
    body{
    background: #EFEFEF;
    }
    @font-face {
    font-family: 'Cherolina';
    src: url('Cherolina.eot');
    src: url('Cherolina.eot?#iefix') format('embedded-opentype'),
        url('Cherolina.woff2') format('woff2'),
        url('Cherolina.woff') format('woff'),
        url('Cherolina.ttf') format('truetype'),
        url('Cherolina.svg#Cherolina') format('svg');
    font-weight: normal;
    font-style: normal;
    font-display: swap;
}

/* THE MAINCONTAINER HOLDS EVERYTHING */
.maincontainer{
  position: absolute;
  width: 380px;
  height: 600px;
  background: none;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-family: sans-serif;
  text-align: center;

}

/* THE CARD HOLDS THE FRONT AND BACK FACES */
.thecard{
  position: relative;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border-radius: 10px;
  transform-style:preserve-3d;
  transition: all 1.5s ease;
}

/* THE PSUEDO CLASS CONTROLS THE FLIP ON MOUSEOVER AND MOUSEOUT */
.thecard:hover{
  transform: rotateY(180deg);
}

/* THE FRONT FACE OF THE CARD, WHICH SHOWS BY DEFAULT */
 .thefront{
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border-radius: 10px;
  backface-visibility: hidden;
  overflow: hidden;
  background: #DAE8EB;
  color: #ffffff;
}

/* THE BACK FACE OF THE CARD, WHICH SHOWS ON MOUSEOVER */
.theback{
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  border-radius: 10px;
  backface-visibility: hidden;
  overflow: hidden;
  background: #fafafa;
  color: #333;
  text-align: center;
  transform: rotateY(180deg);
}


/*This block (starts here) is merely styling for the flip card, and is NOT an essential part of the flip code */
.thefront p{
  font-family: 'Cherolina';
  padding: 30px;
  font-weight: normal;
  font-size: 60pt;
  text-align: center;
  font-style: italic;
  color: #343434ef;
  position: absolute;
  top: -165px;
  left: 50px;
}

.theback h1{
  font-family: sans-serif;
  padding: 30px;
  font-weight: bold;
  font-size: 30px;
  text-align: center;
}

.theback p{
  font-family: 'zilla slab', sans-serif;
  padding: 30px;
  font-weight: normal;
  font-size: 12px;
  text-align: center;
}

.imgtoothless{
    position: relative;
    top: 270px;
}

.imghpbd{
    position: absolute;
    top: 15px;
    right: -45px;
}

/*This block (ends here) is merely styling for the flip card, and is NOT an essential part of the flip code */
    </style>

  <body>
    <div class="maincontainer">
      
      <div class="thecard">

        <div class="thefront">
            <div class="imgtoothless"><img src="https://i.pinimg.com/564x/4b/ac/10/4bac103aa246d90524eb6c96bca25dbb.jpg" width="360px" height="360px"><p>ngkphun</p></div>
            <div class="imghpbd"><img src="hpbd.png" width="450px" height="300px"></div>
        </div>
        <div class="theback"><h1>Back of Card</h1><p>dear</p></div>
        
      </div>
      <p>Tap to read message =))))</p>
    </div>

  </body>
</html>
