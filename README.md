# fun-roulette
shows number visible
html code


<!DOCTYPE html>
<html>
<head>

  <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.11.2/jquery.min.js"></script>
  <script>

  function autoRefresh()
  {
    window.location = window.location.href;
  }

  setInterval('autoRefresh()', 60000); // this will reload page after every 5 secounds; Method I
  </script>
  <script>
    $(document).ready(function () {

        var _str ="";
        var _strTime = 60;

        Time();
        Check();       

        setInterval(function(){ Time(); }, 1000);
        setInterval(function(){ Check(); }, 60000);
               
        function Time()
        {         
           var _strT = "Time Countdown: " + _strTime;
           $("#hdivDisplayTime").html(_strT );
   
           _strTime--;
           if (_strTime < 0)
           {
               _strTime = 60;
           } 
            //alert(_strTime);                       
        }       

        function Check()
        {           
           _str +="<br>";
            var _intI = 0;
            while (_intI < 10) {
                _str += Math.floor((Math.random() * v) + 37;
                $("#hdivDisplayNumbers").html(_str);
                _intI++;
            }
                       
        }
    });
  </script>
  <title></title>
</head>
<body>
  <div id="hdivDisplayTime"></div>
  <div id="hdivDisplayNumbers"></div>
</body>
</html>
