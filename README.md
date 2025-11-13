# NAME: DEEPIKA G
#  REG.NO: 212224040060
# Ex.07 Restuarant Website
## Date: 12-11-2025
## AIM:
To develop a static Resturant website to display the menu and services provided by the resturant.

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
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Play Bae Cafe - Colorful Fusion Cuisine</title>
    <style>
        /* Reset and base styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(45deg, #ff6b6b, #feca57, #48dbfb, #0abde3, #a55eea, #ff9ff3);
            background-attachment: fixed;
            min-height: 100vh;
        }

        /* Header and Navigation */
        header {
            background: rgba(255, 255, 255, 0.9);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
        }

        .logo {
            font-size: 2rem;
            font-weight: bold;
            background: linear-gradient(45deg, #ff6b6b, #feca57);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        nav ul {
            list-style: none;
            display: flex;
        }

        nav ul li {
            margin-left: 2rem;
        }

        nav ul li a {
            text-decoration: none;
            color: #333;
            font-weight: bold;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: #ff6b6b;
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 10rem 2rem 5rem;
            position: relative;
        }

        .hero-img {
            width: 100%;
            height: 400px;
            object-fit: cover;
            border-radius: 10px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.2);
            margin-bottom: 2rem;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            animation: rainbow 3s infinite;
        }

        @keyframes rainbow {
            0% { color: red; }
            16% { color: orange; }
            33% { color: yellow; }
            50% { color: lightgreen; }
            66% { color: rgb(0, 171, 251); }
            83% { color: rgb(255, 15, 255); }
            100% { color: rgb(255, 0, 200); }
        }

        .btn {
            display: inline-block;
            padding: 0.8rem 2rem;
            background: linear-gradient(45deg, #ff6b6b, #feca57);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            transition: transform 0.3s;
        }

        .btn:hover {
            transform: scale(1.1);
        }

        /* Menu Section */
        #menu {
            padding: 4rem 2rem;
            background: rgba(255, 255, 255, 0.9);
            text-align: center;
        }

        .menu-items {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin-top: 2rem;
        }
        .item {
            padding: 2rem;
            margin: 1rem;
            border-radius: 10px;
            width: 300px;
            transition: transform 0.3s;
        }

        
        .item:hover {
            transform: translateY(-10px);
        }

        .item img {
            width: 500%;
            height: 900px;
            object-fit: cover;
            border-radius: 5px;
            margin-bottom: 1rem;
        }

        .price {
            font-weight: bold;
            color: #ff6b6b;
        }

        /* About and Contact Sections */
        #about, #contact {
            padding: 4rem 2rem;
            background: rgba(255, 255, 255, 0.9);
            text-align: center;
        }

        /* Footer */
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 1rem;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            nav ul {
                flex-direction: column;
                margin-top: 1rem;
            }
            nav ul li {
                margin: 0.5rem 0;
            }
            .menu-items {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="logo">Play Bae</div>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#menu">Menu</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="hero">
        <img src="c:\Users\admin\Pictures\Screenshots\Screenshot 2025-11-10 203657.png" alt="Colorful restaurant interior" class="hero-img">
        <h1>Welcome to Play Bae!</h1>
        <p>Where flavors explode in a spectrum of colors. Dive into our creative fusion dishes!</p>
        <a href="#menu" class="btn">Explore Menu</a>
    </section>

    <section id="menu">
        <h2>Our Features</h2>
        <div class="Speciality">
            <div class="Fresh food with games">
                <img src="c:\Users\admin\Pictures\Screenshots\Screenshot 2025-11-10 210127.png">
               
            </div>

             <h3>OUR MENU</h3>
            <div class="item">
                <img src="c:\Users\admin\Downloads\menu.png">
                
               
            </div>
            <div class="item">
                <img src="c:\Users\admin\Downloads\drinks.png">
                
                
            </div>
        </div>
    </section>

    <section id="about">
        <h2>About Us</h2>
        <p>At Plat Bae, we blend cultures and colors to create unforgettable dining experiences. Our chefs experiment with bold flavors and vibrant presentations to make every meal a feast for the senses.</p>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <p>Address: 123 Colorful Lane, Vibrant City<br>
        Phone: 9876543210<br>
        Email: info@playbae.com</p>
    </section>

    <footer>
        <p>&copy; 2025 Play Bae. All rights reserved.</p>
    </footer>
</body>
</html>
```
## OUTPUT:
<img width="1917" height="1140" alt="Screenshot 2025-11-13 085225" src="https://github.com/user-attachments/assets/98f65949-95f2-4083-ae52-d991b55a9b6d" />
<img width="1915" height="1145" alt="Screenshot 2025-11-13 085242" src="https://github.com/user-attachments/assets/57fa8d53-3084-48e0-b7e5-0d6a2cfa71ee" />
<img width="1909" height="1138" alt="Screenshot 2025-11-13 085305" src="https://github.com/user-attachments/assets/3bd0bc75-83b6-4280-8af0-7f4a3088fce9" />
<img width="1919" height="1140" alt="Screenshot 2025-11-13 085255" src="https://github.com/user-attachments/assets/dd4700bd-aea2-4f62-98e4-d1fea51b6032" />

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
