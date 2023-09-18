# Host-website-pages-on-diff.-instances 
Host multiple pages of a single website on different ec2 instances with the help of Application LB.

# Step 1:
 For demonstrating this excersize, Create 3 instances and install apache in it.

 # For Instance 1 : create an index page on its root folder

 cd /var/www/html

 vi index.html
```
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
 # For Instance 2 : create an html page on /contact folder

cd /var/www/html/
mkdir images ; cd images
vi index.html

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

 # For Instance 3 : create an html page on /services folder

cd /var/www/html/
mkdir images ; cd images
vi index.html

```
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
