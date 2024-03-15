# Simple Web Application (docker/flask)
This is a simple web application using python flask to demonstrate Creating Dockerfile and Images for Docker familiarization.

Below are the steps required to get this working on a base linux system (UBUNTU).
Install all required dependencies
Install and Configure Web Server
Start Web Server

1. Install all required dependencies
Python and its dependencies
```
update && apt-get install -y python3 python3-pip
```
3. Install and Configure Web Server
Install Python Flask dependency
```
pip install flask
```
Copy app.py or download it from source repository

3. Start Web Server
Start web server
```
FLASK_APP=/opt/app.py flask run --host=0.0.0.0 --port 8080
```

4. Test
Open a browser and go to URL
if run inside virtual machine
```
http://<IP>:8080                            => Welcome
http://<IP>:8080/how%20are%20you            => I am good, how about you?
```
if run in Docker Desktop
```
localhost:8080
```
