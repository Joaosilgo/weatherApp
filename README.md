

# WeatherApp
 
### Developed by:

João Gomes 


## API

The api used in this project is a one call api from openweathermap.org 

Eg. of use:

https://openweathermap.org/data/2.5/weather?q=Lisboa,pt&appid=439d4b804bc8187953eb36d2a8c26a02

```javascript

document.write("jquery loaded");
        $.getJSON("https://openweathermap.org/data/2.5/weather?q=Lisboa,pt&appid=439d4b804bc8187953eb36d2a8c26a02",function(json){
            document.write(JSON.stringify(json));
        });
```

## HTML Geolocation API

The HTML Geolocation API is used to get the geographical position of a user.

Since this can compromise privacy, the position is not available unless the user approves it.



## Browser Geolocation

```javascript
<script>
var x = document.getElementById("demo");
function getLocation() {
  if (navigator.geolocation) {
    navigator.geolocation.getCurrentPosition(showPosition);
  } else {
    x.innerHTML = "Geolocation is not supported by this browser.";
  }
}

function showPosition(position) {
  x.innerHTML = "Latitude: " + position.coords.latitude +
  "<br>Longitude: " + position.coords.longitude;
}
</script>
```

