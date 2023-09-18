# Host-website-pages-on-diff.-instances 
Host multiple pages of a single website on different ec2 instances with the help of Application LB.

# Step 1:
 For demonstrating this excersize, Create 3 instances and install apache in it.

 # For Instance 1 : create an index page on its root folder

 cd /var/www/html
```
 vi index.html

<html>
<head>
<title>New Website</title>
</head>

<body>

<h1><center>My website</center></h1>

<center><a href="/images/">Images</a></center>
<center><a href="/js/">js</a></center>

</body>

</html>
```

![image](https://github.com/Blesson02/Host-website-pages-on-diff.-instances/assets/108075329/a434a036-f0a9-4fe5-b52a-0f3d67dff0e8)


 # For Instance 2 : create an html page on /contact folder
```
cd /var/www/html/
mkdir images ; cd images
vi index.html
```
```
<html>
<head>
<title>New Website</title>
</head>

<body>
<h1><center>My website</center></h1>

<center><a href="/contacts/">contacts</a></center>

</body>
</html>
```
![image](https://github.com/Blesson02/Host-website-pages-on-diff.-instances/assets/108075329/46e7a388-5bf6-492b-a871-9d2e3a7e6a9b)


 # For Instance 3 : create an html page on /services folder
```
cd /var/www/html/
mkdir images ; cd images
```
```
vi index.html

<html>
<head>
<title>New Website</title>
</head>

<body>
<h1><center>My website</center></h1>

<center><a href="/services/">services</a></center>

</body>
</html>
```
![image](https://github.com/Blesson02/Host-website-pages-on-diff.-instances/assets/108075329/477124f9-d3e0-4b10-910f-3e1456738f74)

## Step 2 : Create Target groups

![image](https://github.com/Blesson02/Host-website-pages-on-diff.-instances/assets/108075329/3df94879-328e-4455-b82e-4e5cf6cb178b)


## Step 3 : Create ALB

![image](https://github.com/Blesson02/Host-website-pages-on-diff.-instances/assets/108075329/24266d6c-c3fb-4d47-955e-56856e22da7f)

## Step 4 : Create rules 

![image](https://github.com/Blesson02/Host-website-pages-on-diff.-instances/assets/108075329/f7e97c9c-e6c8-4287-a0f6-bd6a7888d2ab)

