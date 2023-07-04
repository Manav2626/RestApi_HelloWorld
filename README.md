# RestApi_HelloWorld

This is Python based REST API 
which will give message Hello World on localhost:(given port)/hello


Prerequirements:
1. Install docker
2. Docker should be running 
3. open terminal and change directory to RestApi folder 
4. docker build -t my-flask-rest-api . 
(will download docker image and build docker container for you)
4. docker run -d -p 8000:5000 my-flask-rest-api 
(here I am using port 8000, you can use any, this will run the container on given port)

open browser and write 

localhost:8000/hello    
(replace 8000 with given port if you have changed)

you'll get 

{"message":"Hello, World!"}
