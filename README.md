# Web Page for Mathematical Calculations

## AIM:

To design a static website with validation to perform mathematical calculations in client side.

## DESIGN STEPS:

### Step 1:

Requirement collection.

### Step 2:

Creating the layout using HTML and CSS.

### Step 3:

Write javascript to perform the calculations.

### Step 4:

Include regularexpression based input validation.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
~~~
<!DOCTYPE html>
<html>

<head>
  
  <title>Volume Calculator</title>
</head>

<body>

  <div class="formelement">
    <h1><center><small>Volume Calculator For Cylinder </small></h1></center>
  </div>
  <div class="container">
    <div class="content">
      <h1><center>Volume Of Cylinder</h1></center>
      <form><br><br><br>
        <div class=formelement>
          <lable for="aedit">Height:</lable>
          <input id="aedit" placeholder="" />
          <label><small>
              Meters
            </small></label>
        </div><br>
        <div class=formelement>
          <lable for="bedit">Radius:</lable>
          <input id="bedit" placeholder="" />
          <label><small>
              Meters
            </small></label>
        </div><br>
        <div class=formelement>
          <lable for="cedit">Volume:</lable>
          <input type="number" min="0" value="0" step="any" id="cedit" placeholder="0" readonly="0" /><label><small>
              Meters³</small></label>
        </div><br><br>
        <div class=formelement>
          <input type="button" class="button" value="CALCULATE" id="calbutton1" />
          <input type="Reset" class="button" value="RESET">
        </div>
        <center>
          <p id="stats1"></p>
        </center>
        <br>
        <div class=formula>
          Formula is
          Volume V = π X Radius² X Height
        </div><br>
      </form>
    </div>

    

    
  
</body>
<script type="text/javascript">
  var button;
  button = document.querySelector("#calbutton1");
  button.addEventListener("click", function () {
    var atext, btext, ctext;
    var aval, bval, cval;
    let text1
    atext = document.querySelector("#aedit");
    btext = document.querySelector("#bedit");
    ctext = document.querySelector("#cedit");

    if (Number(atext.value) && Number(btext.value)) {
      aval = parseInt(atext.value);
      bval = parseInt(btext.value);
      text1 = "The Answer Is Generated Successfully!!!";

    }
    

    cval = 3.14 * aval * aval * bval;
    ctext.value = "" + cval;

    document.getElementById("stats1").innerHTML = text1;

  });
</script>


<style>
body{
    background-color: aqua;
}
.container{
    width:1080px;
    margin-left: auto;
    margin-right: auto;
}
.content{
    background-color: beige;
    min-height: auto;
}
.formelement{
    text-align: center;

}
.formula{
    text-align: center;
}
</style>

</html>
~~~
## OUTPUT:
![w1](https://user-images.githubusercontent.com/94154683/149521999-6e64ba08-f95e-42ea-95f0-dde8c6277a9b.PNG)

![w2](https://user-images.githubusercontent.com/94154683/149522038-48815bc1-b432-4f29-a4f2-de8aed938aa9.PNG)






## Result:

Thus a website is designed to perform mathematical calculations in the client side.
