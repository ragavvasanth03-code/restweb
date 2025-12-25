# Ex.07 Restaurant Website
## Date:

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

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

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>RES</title>
  <style>
    body {
      font-family: Arial, sans-serif;
    margin: 0;
      background: #ea2102;
      color: #fff700;
    }
    header {
      background: #ef4b04;
      text-align: center;
      padding: 20px;
    }
    header h1 {
      margin: 0;
      font-size: 25px;
    }
    nav {
      background: #8d8c8c;
      text-align: center;
      padding: 10px 0;
    }
    nav a {
      color: #ffd500;
      text-decoration: none;
      margin: 0 20px;
      font-weight: bold;
    }
    nav a:hover {
      color: #ffcc00;
    }
    .banner {
      background: url('Screenshot 2025-09-29 231228.png') no-repeat center/cover;
      color: rgb(255, 217, 0);
      padding: 60px 20px;
      text-align: center;
    }
    .banner h2 {
      font-size: 30px;
      margin-bottom: 10px;
    }
    .cards {
      display: flex;
      justify-content: space-around;
      margin: 20px;
      gap: 15px;
    }
    .card {
      background: #000000;
      padding: 15px;
      border-radius: 10px;
      width: 30%;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.2);
    }

    .card img {
      width: 100%;
      border-radius: 10px;
      margin-bottom: 10px;
    }
    .footer {
      background: #333;
      color: white;
      text-align: center;
      padding: 15px;
      margin-top: 20px;
    }
    .footer span {
      color: orange;
      font-weight: bold;
    }
    section {
      padding: 20px;
      display: none;
    }
    section.active {
      display: block;
    }
  </style>
  <script>
    function showPage(pageId) {
      let pages = document.querySelectorAll("section");
      pages.forEach(p => p.classList.remove("active"));
      document.getElementById(pageId).classList.add("active");
    }
  </script>
</head>
<body>

<header>
  <h1>🥗 VENIZZ 🥗</h1>
</header>

<nav>
  <a href="#" onclick="showPage('home')">Home</a>
  <a href="#" onclick="showPage('menu')">Menu</a>
  <a href="#" onclick="showPage('admin')">Administration</a>
  <a href="#" onclick="showPage('contact')">Contact Us</a>
</nav>

<!-- Home Section -->
<section id="home" class="active">
  <div class="banner">
    <h2>30% Off This Weekend For You</h2>
    <p>Enjoy delicious meals with special discounts only at Venizz!</p>
    <p>Visit us this weekend and savor the flavors.</p>
    <p><b>Offer valid from Friday to Sunday.</b></p>
  </div>

  <div class="cards">
    <div class="card">
      <h3>Our New Menu</h3>
      <img src="image.png" alt="Menu">
      <p>Check out our fresh and tasty new dishes for this season.</p>
    </div>
    <div class="card">
      <h3>Book a Table</h3>
      <img src="table .png"alt="Table">
      <p>Reserve your table easily and enjoy dining with us.</p>
    </div>
    <div class="card">
      <h3>Opening Hours</h3>
      <img src="time.png" alt="Hours">
      <p>Mon–Fri: 10am - 10pm<br>Sat: 11am - 1am<br>Sun: 2pm - 12am</p>
    </div>
  </div>
</section>
<!-- Menu Section -->
 <body style="background-color:#b71304;">

<section id="menu" style="text-align:center;">

<h2 style="color:yellow; font-size:36px; letter-spacing:3px;">
OUR MENU
</h2>

<table style="margin:auto;" cellpadding="20">

<tr>
<td>
<div style="background:black; width:230px; height:360px; border-radius:25px; padding:15px;">
<img src="Grill.png"
style="width:200px; height:200px; object-fit:cover; border-radius:20px;">
<p style="color:yellow; font-size:22px; font-weight:bold; margin-top:12px;">
Grill Chicken
</p>
<p style="color:white; font-size:20px; font-weight:bold;">
₹300
</p>
</div>
</td>

<td>
<div style="background:black; width:230px; height:360px; border-radius:25px; padding:15px;">
<img src= "veg salad.png"
style="width:200px; height:200px; object-fit:cover; border-radius:20px;">
<p style="color:yellow; font-size:22px; font-weight:bold; margin-top:12px;">
Veg Salad
</p>
<p style="color:white; font-size:20px; font-weight:bold;">
₹150
</p>
</div>
</td>

<td>
<div style="background:black; width:230px; height:360px; border-radius:25px; padding:15px;">
<img src="chicken pizza .png"
style="width:200px; height:200px; object-fit:cover; border-radius:20px;">
<p style="color:yellow; font-size:22px; font-weight:bold; margin-top:12px;">
Chicken Pizza
</p>
<p style="color:white; font-size:20px; font-weight:bold;">
₹450
</p>
</div>
</td>
</tr>

<tr>
<td>
<div style="background:black; width:230px; height:360px; border-radius:25px; padding:15px;">
<img src="white sause .png"
style="width:200px; height:200px; object-fit:cover; border-radius:20px;">
<p style="color:yellow; font-size:22px; font-weight:bold; margin-top:12px;">
White Sauce Pasta
</p>
<p style="color:white; font-size:20px; font-weight:bold;">
₹200
</p>
</div>
</td>
<td>
<div style="background:black; width:230px; height:360px; border-radius:25px; padding:15px;">
<img src="cheese burger .png"
style="width:200px; height:200px; object-fit:cover; border-radius:20px;">
<p style="color:yellow; font-size:22px; font-weight:bold; margin-top:12px;">
Cheeseburger
</p>
<p style="color:white; font-size:20px; font-weight:bold;">
₹100
</p>
</div>
</td>

<td>
<div style="background:black; width:230px; height:360px; border-radius:25px; padding:15px;">
<img src="fish curry.png"
style="width:200px; height:200px; object-fit:cover; border-radius:20px;">
<p style="color:yellow; font-size:22px; font-weight:bold; margin-top:12px;">
Fish Curry
</p>
<p style="color:white; font-size:20px; font-weight:bold;">
₹150
</p>
</div>
</td>
</tr>

<tr>
<td>
<div style="background:black; width:230px; height:360px; border-radius:25px; padding:15px;">
<img src="chicken.png"
style="width:200px; height:200px; object-fit:cover; border-radius:20px;">
<p style="color:yellow; font-size:22px; font-weight:bold; margin-top:12px;">
Chicken Biryani
</p>
<p style="color:white; font-size:20px; font-weight:bold;">
₹250
</p>
</div>
</td>

<td>
<div style="background:black; width:230px; height:360px; border-radius:25px; padding:15px;">
<img src= "prawn.png"
style="width:200px; height:200px; object-fit:cover; border-radius:20px;">
<p style="color:yellow; font-size:22px; font-weight:bold; margin-top:12px;">
Prawn Fry
</p>
<p style="color:white; font-size:20px; font-weight:bold;">
₹200
</p>
</div>
</td>

<td>
<div style="background:black; width:230px; height:360px; border-radius:25px; padding:15px;">
<img src="tandoori paneer .png"
style="width:200px; height:200px; object-fit:cover; border-radius:20px;">
<p style="color:yellow; font-size:22px; font-weight:bold; margin-top:12px;">
Tandoori Paneer
</p>
<p style="color:white; font-size:20px; font-weight:bold;">
₹180
</p>
</div>
</td>
</tr>

</table>

</section>

</body>





<!-- Administration Section -->
<section id="admin">
  <h2>Administration</h2>
  <ul>
    <li>Kishoth – Manager</li>
    <li>Sanjay – Chef</li>
    <li>Lokesh – Assistant Chef</li>
    <li>Shiva  – Waitress</li>
    <li>Rahman  – Waiter</li>
    <li>Vishnu – Cashier</li>
  </ul>
</section>

<!-- Contact Section -->
<section id="contact">
  <h2>Contact Us</h2>
  <p><b>Address:</b> 1st,Anna Nagar,chennai,India </p>
  <p><b>Phone:</b> +91 8110838422  </p>
  <p><b>Email:</b> info@evec.com </p>
</section>

<!-- Footer -->
<div class="footer">
  Designed and Developed by <span> V.Ragavan 25018843 </span>
</div>

</body>
</html>
```


## OUTPUT:
<img width="1919" height="1025" alt="image" src="https://github.com/user-attachments/assets/ee9f18ed-583e-47df-a490-2541b8610638" />
<img width="1919" height="1016" alt="image" src="https://github.com/user-attachments/assets/b3d93217-aeda-4ca5-8042-5106d286245f" />
<img width="1917" height="1024" alt="image" src="https://github.com/user-attachments/assets/24b42ad8-d245-4a2a-877a-68f9aca9d612" />
<img width="1919" height="1023" alt="image" src="https://github.com/user-attachments/assets/04b5d841-9401-4079-89b3-c4b6f7f81c7e" />



## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
