# Ex04 Places Around Me
## Date: 11-04-2024

## AIM
To develop a website to display details about the places around my house.

## DESIGN STEPS

### STEP 1
Create a Django admin interface.

### STEP 2
Download your city map from Google.

### STEP 3
Using ```<map>``` tag name the map.

### STEP 4
Create clickable regions in the image using ```<area>``` tag.

### STEP 5
Write HTML programs for all the regions identified.

### STEP 6
Execute the programs and publish them.

## CODE

```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    *{margin: 0;}
</style>
<script>
    function coordinate(event){
        let x=event.clientX;
        let y=event.clientY;
        document.getElementById("text1").value=x;
        document.getElementById("text2").value=y;
    }
</script>
<body>
    <img src="map.png" width="1500" height="650" usemap="#MapNew" onmousemove="coordinate(event)">
    <MAP name="MapNew">
        <area shape="rect" coords="198,294,240,313" href="https://apolloartsandsciencecollegechennai.ac.in/" Title="Apollo Arts And Science" >
        <area shape="rect" coords="297,330,380,393" href="https://www.saveetha.ac.in/" Title="Saveetha Engineering College" >
        <area shape="rect" coords="943,117,1000,184" href="https://sapoly.edu.in/" Title="SA Polytechnic College" >
        <area shape="rect" coords="1152,280,1227,328" href="https://www.sriramachandra.edu.in/" Title="Sri Ramachandra Hospitals" >
        <area shape="rect" coords="928,10,1005,13" href="https://www.mahalakshmi.edu.in/" Title="Mahalakshmi Women's College" >
        <area shape="rect" coords="1143,211,1209,254" href="https://www.alphagroup.edu.in/" Title="Alpha Arts And Science College" >

    </MAP>
    <br>
    X coordinator
    <input type="text" id="text1">
    <br>
    Y coordinate
    <input type="text" id="text2">
</body>
</html>

```

## OUTPUT

![Screenshot (21)](https://github.com/thejaswinidhanaraj/NearMe/assets/148514511/b65d9a3d-d2c4-4e64-b8b9-2dc29e0bb986)

## RESULT
The program for implementing image maps using HTML is executed successfully.
