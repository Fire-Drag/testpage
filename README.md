# testpage
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" type="text/css"  href="final1.css"/>
    

    </head>
        <body>
            <center> <h3>PRESSURE AND TEMPRATURE VARIATIONS WITH CHANGES IN ALTITUDE</h3> </center>
         <div class="nvbar">
             <a href="file:///C:/Users/veena/Desktop/HTML/FINAL%20PROJECT.html">HOME</a>
             <a href="file:///C:/Users/veena/Desktop/HTML/team.html">ABOUT</a>
             <a href="file:///C:/Users/veena/Desktop/SUMMARYREPORT.htm">SUMMARYREPORT</a>
             <a href="https://www3.nd.edu/~nsl/Lectures/phys20054/15Lecture%206%20Atmosphere%20and%20Climate-1.pdf">REFERENCE</a>
             <a href="file:///C:/Users/veena/Desktop/HTML/contact.html">CONTACT</a>
         </div>

        </body>
        <body>
            <table>
                <table style = "width:85% ;height:80%" table align = "center" padding= "40px">
            <tr>
                <td>
                    <h1><ins><b>CALCULATOR:</b></ins></h1>
                </td>
            </tr>
            <tr>
                <td>
                    <center><img src="calculations (3).jpeg" alt="image" width="1400px"; height="400px"></center>
                </td>
            </tr>
            <tr>
                <td>
                   <h1><ins>Enter Altitude From Sea Level Here :</ins></h1>
                   <h2><label for="altitude">(Altitude is the Height Above Sea Level in Meters):</label></h2>
                    <input type="number" id="Height" name="" style="width: 16%; font-weight: 600;font-size: 20px;border-radius: 0cm; border-style: solid" >METERS<br><br>
                </td>
            </tr><br>
            <td>
                <button onclick="calculate()" style="width: 12%; color: snow; background-color: black; font-weight: 600;font-size: 20px;"> SUBMIT </button><br><br>
                <a href="file:///C:/Users/veena/Desktop/HTML/FINAL%20FRONTEND.html"><button style="width: 12%; color: snow; background-color: black; font-weight: 600;font-size: 20px;" >RESET </button></a>
            </td>
            <tr>
                <td>
                   <h1><ins>The Tempreture At Entered Altitude :</ins></h1> 
                   <h2><label for="temperature">(Temperature is in Degree Celsius '°C' ):</label></h2>
                   <p id="RESULT1"  placeholder="RESULT 1" style="width: 12%; font-weight: 600;font-size: 20px;border-radius: 0cm; border-style: solid" ></p>
                </td>
            </tr>
            <tr>
                <td>
                    <h1><ins>The Pressure At Entered Altitude :</ins></h1>
                    <h2><label for="pressure">(Pressure is in KiloPascals 'kPa' ):</label></h2>
                    <p id="RESULT2" type="text" placeholder="RESULT 2" style="width: 12%; font-weight: 600;font-size: 20px; border-radius: 0cm; border-style: solid" ></p>
                </td>
            </tr>
            <script>
                function calculate()
                {
                    var Height = document.getElementById('Height').value;
                    
                    var RESULT1 = document.getElementById('RESULT1').value = 20 - (0.0065*parseFloat(Height)); 
                        document.getElementById('RESULT1').innerHTML = RESULT1 +" °C" ;
   
                    var RESULT2 = document.getElementById('RESULT2').value = 101.325*(1-((0.0065*parseFloat(Height))/(parseFloat(RESULT1)+(0.0065*parseFloat(Height))+273.15)))**5.257;
                        document.getElementById('RESULT2').innerHTML = RESULT2 +" kPa";
                    console.log(RESULT2)
                }
            </script>
            <tr>
                <td>
                  <img src="altitude.png"   alt="image" style=" width:500px ; height: 500px ; padding:60px ">
                  <img src="temperature-icon-stock-gif.gif" alt="gif" style="width:650px; height:450px; padding:100px">
                </td>
                </tr>
            <tr>
                <td>
                    <p>
                       <b><ins>>DESCRIPTION:</ins></b><br><br>
                1) THIS WEBPAGE MEASURES TEMPRETURE AND PRESSURE AT THE ALTITUDE FROM SEA LEVEL ENTERED BY USER IN METER.<br><br>
                2) ENTER ALTITUDE FROM THE THE SEA LEVEL IN THE BELOW INPUT BOX AND WE WILL GIVE YOU CORRESPONDING TEMP AND PRESSURE AT THAT POINT.<br><br>
                3) PRESSURE DECREASES WITH INCREASING ALTITUDE.<br><br>
                4) THE PRESSURE AT ANY LEVEL IN THE ATMOSPHERE MAY BE INTERPRETED AS THE TOTAL WEIGHT OF THE AIR ABOVE A UNIT AREA AT ANY ELEVATION.<br><br>
                5) AT HIGHER ELEVATIONS, THERE ARE FEWER AIR MOLECULES ABOVE A GIVEN SURFACE THAN A SIMILAR SURFACE AT LOWER LEVELS.<br><br>
                6) WHAT THIS IMPLIES IS THAT ATMOSPHERIC PRESSURE DECREASES WITH INCREASING HEIGHT.<br><br>
                7) SINCE MOST OF THE ATMOSPHERE'S MOLECULES ARE HELD CLOSE TO THE EARTH'S SURFACE BY THE FORCE OF GRAVITY, AIR PRESSURE DECREASES RAPIDLY AT FIRST, THEN MORE SLOWLY AT HIGHER LEVELS.<br><br>
                8) TEMPERATURES DECREASE WITH ALTITUDE IN THE TROPOSPHERE AT A RATE OF ABOUT 6.5 DEGREES CELSIUS (11.7 DEGREES FAHRENHEIT) PER KILOMETER, DEPENDING ON THE WEATHER. <br><br>
                9) THIS OCCURS AS A RESULT OF DECREASING AIR PRESSURE WITH ALTITUDE. AS PRESSURE DECREASES, AIR EXPANDS, AND IT COOLS AS IT DOES SO.<br><br>
                </p>
                </td>
            </tr>
        </table>

        </body>
</html>
