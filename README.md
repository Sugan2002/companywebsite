# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Diamond Private Limited</title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel = "icon" href ="{% static 'img/titleicon.png' %}" type = "image/x-icon"> 
              
</head>

<body>
    <div class="container">
    <div class="banner">
        Diamond Private Limited.
    </div>
    <div class="menu">
        <div class="menuitem"><a href="/home">home</a></div> 
        <div class="menuitem"><a href="/ourproducts">Our Products</a></div> 
        <div class="menuitem"><a href="/people">Know The People</a></div>
        <div class="menuitem"><a href="/contact">Contact Us</a></div> 
    </div><div class="content">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="footer">
        Copyright © 2020 Diamond Private Limited, Developed by Suganya Parthiban.
    </div>
    </div>
</body>

</html>
```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
    <h1>What We Do</h1>
    <img src="/static/img/building2.jpeg" alt="Building">
    <div class="contenttext">
    Diamond Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications for its products include: data center networking, home connectivity, broadband access, telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and alternative energy systems, displays, and mainframe operations and management, and application software development. Some of Diamond's core technologies and products include:
    <ul>
        <li>Memory Chips</li>
        <li>SATA HDD</li>
        <li>SATA SSD </li>
        <li>Broadband Modems</li>
        <li>Wifi Devices</li>
        <li>Switching Devices</li>
        <li>Optical Sensors</li>
    </ul> 
    </div>
    </div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="productcontent">    
    <h1>Our Premium Products</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c1.jpg" alt="product image">
            </div>
            <div class="itemname">4GB DDRA4 laptop memory</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c2.jpg"  alt="product image">
            </div>
            <div class="itemname">1TB Laptop HDD</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/black-adsl-modem-with-3-antennae.jpg"  alt="product image">
            </div>
            <div class="itemname">Boardband Modem</div>
            <div class="itemprice">Price: Rs.1,700.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/ssd.jfif"  alt="product image">
            </div>
            <div class="itemname">1TB Laptop ssd</div>
            <div class="itemprice">Price: Rs.1500.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/tube.jpg"  alt="product image">
            </div>
            <div class="itemname">silicon tubes</div>
            <div class="itemprice">Price: Rs.790.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/sheet.jpg"  alt="product image">
            </div>
            <div class="itemname">silicon sheet</div>
            <div class="itemprice">Price: Rs.500.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/watch.jfif"  alt="product image">
            </div><div class="itemname">watch</div>
            <div class="itemprice">Price: Rs.500.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/battry.jfif"  alt="product image">
            </div><div class="itemname">silicon battry</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/switch.jfif"  alt="product image">
            </div><div class="itemname">switch</div>
            <div class="itemprice">Price: Rs.300.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/spray.png"  alt="product image">
            </div><div class="itemname">silicon sparay</div>
            <div class="itemprice">Price: Rs.950.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/microchip.jfif"  alt="product image">
            </div><div class="itemname">micro chip</div>
            <div class="itemprice">Price: Rs.500.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/optical.jfif"  alt="product image">
            </div><div class="itemname">optial lence</div>
            <div class="itemprice">Price: Rs.1500.00 </div>
        </div>
    </div>
    </div>
{% endblock  %}
```

### people.html
```
{% extends "website/base.html" %}

{% block content %}
 <div class="productcontent">    
    <h1>our peoples</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/forbe.jfif" alt="product image">
            </div>
            <div class="itemname">FORBE</div>
            <div>ceo</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/sachin.jfif"  alt="product image">
            </div>
            <div class="itemname">sachin</div>
            <div>sales exclutive</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/viswa.jfif"  alt="product image">
            </div>
            <div class="itemname">vishwanathan anand</div>
            <div>manager</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/dhoni.jfif"  alt="product image">
            </div>
            <div class="itemname">dhoni</div>
            <div>assitant manager</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/mukeshambani.jfif"  alt="product image">
            </div>
            <div class="itemname">mukeshamboney</div>
            <div>md</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/kalanidhi.jfif"  alt="product image">
            </div>
            <div class="itemname">kalanidhi</div>
            <div>production department</div>
        </div>
    </div>
    </div>
{% endblock  %}

```

### contact.html
```
{% extends "website/base.html" %}

{% block content %}
<div class="content">
    <h1>CONTACT US</h1>
    <div class="contacttext">
        <h2>Aazhiya(General Contact Manager)</h2>
        <h2>Arihant diamond Products Private Limited</h2>
        <h2>Arihant diamond Products India Contact Information,Email Address,Main Office Location Including
headquaters address,office phone number,customer support helpline number and email id is available here 
with company bio data,network presence,as well as service locations </h2>
        <h2>Chennai,India - 6000051</h2>
        <h2>contact number - 8362891743</h2>
        <h2>Email address - diamondcompanyrj@gmail.com</h2>
    </div>
</div>
{% endblock %}


```
## OUTPUT:
![output](./static/img/o1.png)

![output](./static/img/o2.png)

![output](./static/img/o3.png)

![output](./static/img/o4.png)

## CODE VALIDATION REPORT:
![output](./static/img/r1.png)

![output](./static/img/r2.png)

![output](./static/img/r3.png)
## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://suganya.student.saveetha.in:8000/. HTML code is validated.