<!DOCTYPE html>
<html>
<head>
  <title>Donate Food</title>
  <link rel="stylesheet" href="style.css">
</head>
<style>
  h1{
    font-size: 30px;
    font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    transform: translateX(1%);
    text-shadow: 2px 2px rgb(173, 222, 222);
  }
  .hi{
    font-family: cursive;
  }
  body {
    margin: auto;
    font-family: -apple-system, BlinkMacSystemFont, sans-serif;
    overflow: auto;
    background: linear-gradient(315deg, rgb(223, 111, 215) 3%, rgb(79, 144, 209) 38%, rgb(89, 200, 192) 68%, rgb(220, 106, 106) 98%);
    animation: gradient 15s ease infinite;
    background-size: 400% 400%;
    background-attachment: fixed;
}

@keyframes gradient {
    0% {
        background-position: 0% 0%;
    }
    50% {
        background-position: 100% 100%;
    }
    100% {
        background-position: 0% 0%;
    }
}

.wave {
    background: rgb(255 255 255 / 25%);
    border-radius: 1000% 1000% 0 0;
    position: fixed;
    width: 200%;
    height: 12em;
    animation: wave 10s -3s linear infinite;
    transform: translate3d(0, 0, 0);
    opacity: 0.8;
    bottom: 0;
    left: 0;
    z-index: -1;
}

.wave:nth-of-type(2) {
    bottom: -1.25em;
    animation: wave 18s linear reverse infinite;
    opacity: 0.8;
}

.wave:nth-of-type(3) {
    bottom: -2.5em;
    animation: wave 20s -1s reverse infinite;
    opacity: 0.9;
}

@keyframes wave {
    2% {
        transform: translateX(1);
    }

    25% {
        transform: translateX(-25%);
    }

    50% {
        transform: translateX(-50%);
    }

    75% {
        transform: translateX(-25%);
    }

    100% {
        transform: translateX(1);
    }
}
select {
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 10 6'><polygon points='0,0 10,0 5,6'/></svg>");
  background-repeat: no-repeat;
  background-position: right 10px center;
  background-size: 6px 4px;
  padding-right: 20px;
}
select {
  border: none;
  border-radius: 20px;
  padding: 10px;
  background-color:azure;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  cursor: pointer;
  overflow: hidden;
}

select::-ms-expand {
  display: none;
}

select::-moz-focus-inner {
  border: 0;
  padding: 0;
}

select option {
  background-color:azure;
}
.round-input {
  border: none;
  border-radius: 25px;
  padding: 10px;
  width: 530px;
  box-shadow: 0px 0px 5px rgba(0,0,0,0.1);
  background-color:azure;
}
label{
  transform: translateY(20%);
}
textarea {
  background-color: rgba(254, 254, 254, 0);
}
textarea {
  opacity: 6;
}
a{
  font-size:35px;
  text-decoration:none;
  text-align: center;
}

</style>
<body>
  <div>
    <div class="wave"></div>
    <div class="wave"></div>
    <div class="wave"></div>
  
  <div class="hi">
  <h1>DONATION DETAILS</h1>
  <form action="submit.php" method="post">
    <label for="donation_type"><b>DONOTION TYPE-</b></label>
    <select name="donation_type">
      <option value="rice">RICE</option>
      <option value="meals">MEALS</option>
      <option value="clothes">CLOTHES</option>
      <option value="curries">CURRIES</option>
      <option value="Medicines">MEDICINES</option>
      <option value="other">OTHER</option>
    </select>
    <br>

    <label for="quantity"><b>QUANTITY-</b></label>
    <input type="number" name="quantity" class="round-input">
<br>
    <label for="unit"><B>UNIT-</B></label>
    <select name="unit">
      <option value="cans">CANS</option>
      <option value="boxes">BOXES</option>
      <option value="bags">BAGS</option>
      <option value="pounds">POUNDS</option>
      <option value="stripes">NO OF STRIPES</option>
      <option value="other">OTHER</option>
    </select>
<br>

<label for="loc"><B>LOCATION-</B></label> <br>
<textarea name="hello" id="loc"  rows="6" cols="60"></textarea>
  </div>
</form>
  <div style="text-align:center; padding:15px;font-size:20px; font-family: cursive;">
    <a href="donate.html" style="color:rgb(25, 27, 25);"><B>DONATE--></B></a>
  </div>
  </div>
</body>
</html>
