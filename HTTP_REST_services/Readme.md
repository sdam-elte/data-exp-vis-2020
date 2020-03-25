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

A **REST service** should always have a detailed documentation, otherwise there is no way for the client to learn it's functionalities. Here are two neat examples:
* Airvisual https://www.iqair.com/air-pollution-data-api
and
 * Chembl https://www.ebi.ac.uk/chembl/api/data/docs

**Airvisual** hosts physical and chemical parameters of the atmosphere collected with vast amount of sensors from all over the world. The API is partially public, clients need to register and obtain a key, with which they authenticate themselves

**Chembl** is a service of the EBI (www.ebi.ac.uk), which serves data from a database, where all sorts of information is stored about chemical/molecular interactions.

### How to build a REST API in python - Tutorials
Please read these tutorials for a deeper understanding of the whole process and for motivation as well:
 * flask
https://blog.miguelgrinberg.com/post/designing-a-restful-api-with-python-and-flask
 * jupyter notebook
https://www.pybloggers.com/2016/01/jupyter-notebooks-as-restful-microservices/

### Examples

In the folder you'll find `REST_API_example_server.ipynb` and `REST_API_example_client.ipynb` that showcases how a REST service can be setup using jupyter notebook with client side code for testing.

When running the server in the terminal with
``` bash
preview-nb-api.sh REST_API_example_server.ipynb
```
the first line in the output will tell you the url of the service (it is the same as with the bokeh server). The url ends with `/report`. If you run your service then the help endpoint should be either at `/report/help` or at `/report/api/help`

### Assignment

You will find the description of the task in the `API-worksheet.ipynb` notebook.

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
If you save this code (maybe replacing the url, with your API server's url) into an HTML file, then loading it to the browser should reveal the button, which then will reveal the returned message. The `button` can be replaced with an `onload` function, which runs immediately when opening the page.