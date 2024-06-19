<html>
<html lang="en">
<head>

 <!-- Google Tag Manager -->
<script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
})(window,document,'script','dataLayer','GTM-MST4ZVS5');</script>
<!-- End Google Tag Manager -->

    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adventure Travel Website</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-image: url('https://image.slidesdocs.com/responsive-images/background/color-blue-nature-travel-agency-fashion-travel-powerpoint-background_2753391815__960_540.jpg');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            background-attachment: fixed;
        }
        header {
            background-color: #B8A983;
            color: white;
            padding: 10px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            flex-wrap: wrap;
            
        }
        header img {
            height: 50px;
        }
        nav ul {
            list-style: none;
            padding: 0;
            display: flex;
            gap: 10px;
            margin: 0;
        }
        nav ul li {
            display: inline;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            cursor: pointer;
            padding: 5px 10px;
            transition: background-color 0.3s;
        }
        nav ul li a:hover {
            background-color: #555;
        }
        main {
            padding: 20px;
        }
        footer {
            background-color: #B8A983;
            color: white;
            text-align: center;
            padding: 10px 20px;
            position: fixed;
            width: 50%;
            bottom: 0;
        }
        .section {
            display: none;
        }
        .section.active {
            display: block;
        }
        @media (max-width: 600px) {
            header {
                flex-direction: column;
                align-items: flex-start;
            }
            nav ul {
                flex-direction: column;
                width: 100%;
            }
            nav ul li {
                width: 100%;
            }
            nav ul li a {
                display: block;
                width: 100%;
                text-align: center;
            }
        }
    </style>
</head>
<body class="body_nav">

 <!-- Google Tag Manager (noscript) -->
<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-MST4ZVS5"
height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
<!-- End Google Tag Manager (noscript) -->

    <header>
        <img src="https://static.vecteezy.com/system/resources/thumbnails/023/404/384/small/adventure-quote-and-so-the-adventure-begins-png.png" alt="Adventure Logo">
        <nav class="header_nav">
            <ul>
                <li><a href="#" onclick="showSection('home')">Home</a></li>
                <li><a href="#" onclick="showSection('next-destination')">Destination</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <div id="home" class="section active">
            <h2>Home Page</h2>
            <p>Welcome to our Adventure Travel Website. Discover amazing places and plan your next adventure with us.</p>
                  <div class="gallery">
                <a href="#" onclick="showSection('singapore')"><img src="https://assets.bwbx.io/images/users/iqjWHBFdfxIU/il7jc87wZ_o8/v0/-1x-1.jpg" alt="Singapore"></a>
                <a href="#" onclick="showSection('hongkong')"><img src="https://cdn.pixabay.com/photo/2020/12/17/00/43/skyscrapers-5838029_1280.jpg" alt="Hong Kong"></a>
                <!-- Add more images as needed -->
            </div>
        </div>
        <div id="next-destination" class="section">
            <h2>Next Destination</h2>
            <p>Our next exciting destination is the beautiful beaches of Bali, Indonesia. Join us for an unforgettable adventure!</p>
            <ul>
                <li>Explore stunning beaches</li>
                <li>Experience vibrant culture</li>
                <li>Enjoy delicious cuisine</li>
                <li>Relax in luxurious accommodations</li>
            </ul>
        </div>

       <div id="singapore" class="section">
            <h2>Singapore</h2>
            <p>OEnjoy Singapore!</p>
        </div>

         <div id="hongkong" class="section">
            <h2>HongKong</h2>
            <p>Enjoy HongKong!</p>
        </div>
    </main>
    <footer">
        <p class="footer_nav">&copy;Adventure Travel Website. <a href="#" onclick="showSection('next-destination')">Destination</a></p>
        
    </footer>
    <script>
        function showSection(sectionId) {
            const sections = document.querySelectorAll('.section');
            sections.forEach(section => {
                section.classList.remove('active');
            });
            document.getElementById(sectionId).classList.add('active');
        }
    </script>
</body>
</html>
