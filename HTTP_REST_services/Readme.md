## HTTP protocol

Here are some tutorial videos:
 * https://www.youtube.com/watch?v=k6fy7mvNSnY
 * https://www.youtube.com/watch?v=iYM2zFP3Zn0
 * https://www.youtube.com/watch?v=JFZMyhRTVt0

or take a look at these sites for further informations:
 * https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol
 HTTP functions as a request–response protocol in the client–server computing model
 * https://www.ntu.edu.sg/home/ehchua/programming/webprogramming/HTTP_Basics.html


## REST services

The basics of it are explained in these videos:
 * https://www.youtube.com/watch?v=LooL6_chvN4
 * https://www.youtube.com/watch?v=7YcW25PHnAA
 * https://www.youtube.com/watch?v=Q-BpqyOT3a8


https://www.ntu.edu.sg/home/ehchua/programming/webprogramming/HTTP_Basics.html

### Transferring images - some help

You can only send text via the api. So if you want to send an image then i the data needs to be converted to text, then download it and convert back to image.

curl https://kooplex-edu.elte.hu/notebook/wfct0p-dataexplvisu/report/img > img.png

And this is how you convert it back to png
``` python
import base64
import json

with open("img.png",'r') as i:
    imgstr = json.loads(i.read())
    img_encoded = base64.decodebytes(imgstr.encode())

    # Then maybe write it to a file
    with open("t.png",'wb') as t:
        t.write(img_encoded)
```

### With jQuery and javascript 
it is possible to send a request to an API, transfer the data and update your webpage. Here is code snippet, that will do it.

```
<!DOCTYPE html>
<html>
<head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
<script>
$(document).ready(function(){
  $("button").click(function(){
    $.get("https://kooplex-fiek.elte.hu/notebook/wfct0p-rere-wfct0p/report/help", function(data, status){
      $("#test1").html(data);
    });
  });
});
</script>
</head>
<body>

<button>Send an HTTP GET request to the API and get the result back</button>
<p id=test1></p>
</body>
</html>
```
Try the following button:

<!DOCTYPE html>
<html>
<head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
<script>
$(document).ready(function(){
  $("button").click(function(){
    $.get("https://kooplex-fiek.elte.hu/notebook/wfct0p-rere-wfct0p/report/help", function(data, status){
      $("#test1").html(data);
    });
  });
});
</script>
</head>
<body>

<button>Send an HTTP GET request to the API and get the result back</button>
<p id=test1></p>
</body>
</html>