# 504jayfinalexam
Steps to build website on EC2 using Git hub Action.
1) Create Github Repository
2) make workflow file and write .yml code to build web server and add static flles  in /var/www/html folder
3) Create Docker file in same directory where all files are exist.
4)Install docker on EC2
5) Build Docker Image
6) Deploy image on Docker Registory
7) Run Docker Container to deploy website.
    sudo docker run -d -p 5000:80 jaypatel132/504finalexam:v1.0
