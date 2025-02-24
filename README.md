<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Real Estate</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <nav class="navbar">
        <a href="#" class="nav-logo">
            <h2 class="logo-text">Real Estate</h2>
        </a>
        <ul class="nav-menu">
            <li class="nav-item"><a href="#" class="nav-link">Home</a></li>
            <li class="nav-item"><a href="Aboutus.html" class="nav-link">About</a></li>
            <li class="nav-item"><a href="#" class="nav-link">Properties</a></li>
            <li class="nav-item"><a href="#" class="nav-link">Buy/Rent</a></li>
            <li class="nav-item"><a href="Contact.html" class="nav-link">Contact Us</a></li>
            <li><button class="btnlogin-popup"id="loginBtn">Login</button></li>            
        </ul>
    </nav>
</header>

<main>
    <section class="hero-section">
        <div class="section-content">
            <div class="hero-details">
                <h2 class="title">Find Your Dream Home</h2>
                <section class="center">
                    <form action="search.html" method="post">
                        <h3>FIND YOUR PERFECT HOME</h3>
                        <div class="box">
                            <p>Enter Location <span>*</span></p>
                            <input type="text" name="location" required maxlength="50" placeholder="Enter city name" class="input">
                        </div>
                        <div class="flex">
                            <div class="box">
                                <p>Property Type <span>*</span></p>
                                <select name="type" class="input" required>
                                    <option value="flat">Flat</option>
                                    <option value="house">House</option>
                                    <option value="land">Land</option>
                                </select>
                            </div>
                            <div class="box">
                                <p>Select City <span>*</span></p>
                                <select name="place" class="input" required>
                                    <option value="Kathmandu">Kathmandu</option>
                                    <option value="Lalitpur">Lalitpur</option>
                                    <option value="Bhaktapur">Bhaktapur</option>
                                </select>
                            </div>
                            <div class="box">
                                <p>Minimum Budget <span>*</span></p>
                                <select name="budget" class="input" required>
                                    <option value="200000-500000">20K-50K</option>
                                    <option value="1000000-2000000">1Lac-2Lac</option>
                                    <option value="10000000-500000000">1Crore-5Crore</option>
                                </select>
                            </div>
                        </div>
                        <input type="submit" value="Search Property" name="search" class="btn">
                    </form>
                </section>
            </div>
        </div>
    </section>
    

<div id="loginModal" class="modal">
  <div class="modal-content">
    <span class="close">&times;</span>
    <form class="login-form">
      <h2>Login</h2>
      <div class="form-group">
        <label for="email">Email</label>
        <input type="email" id="email" name="email" required>
      </div>
      <div class="form-group">
        <label for="password">Password</label>
        <input type="password" id="password" name="password" required>
       </div>      
        <div class="show-password">  
        <input type="checkbox" id="showPassword">
        <label for="showPassword">Show Password</label>
      </div>
      <button type="submit" class="btn-login">Login</button>
      <p class="extra-linl">Don’t have an account? <a href="#">Register</a></p>
    </form>
  </div>
</div>

<section class="properties" id="properties">
    <div class="title-box">
        <h2 class="section-title">LATEST LISTING</h2>
    </div>
    <p class="section-description">
        Discover stunning homes that match your dreams and budget. From cozy apartments to luxurious villas, 
        find the perfect space to call home.
    </p>

    <div class="property-grid">
        <!-- First three listings (visible by default) -->
        <div class="property-card">
            <img src="home2.webp" alt="Modern House">
            <h3>RS 2,50,00,000</h3>
            <p>Kathmandu</p>
            <a href="#" class="view-property-btn">View Property</a>
        </div>
        <div class="property-card">
            <img src="home3.jpg" alt="Luxury Villa">
            <h3>RS 12,00,00,000</h3>
            <p>Pokhara</p>
            <a href="#" class="view-property-btn">View Property</a>
        </div>
        <div class="property-card">
            <img src="home1.jpg" alt="City Apartment">
            <h3>RS 3,50,00,000</h3>
            <p>Bhaktapur</p>
            <a href="#" class="view-property-btn">View Property</a>
        </div>

        <!-- Hidden properties (shown after clicking "View All") -->
        <div class="property-card hidden">
            <img src="home4.jpg" alt="Suburban Home">
            <h3>RS 4,50,00,000</h3>
            <p>Lalitpur</p>
            <a href="#" class="view-property-btn">View Property</a>
        </div>
        <div class="property-card hidden">
            <img src="home5.webp" alt="Cozy Cottage">
            <h3>RS 1,80,00,000</h3>
            <p>Biratnagar</p>
            <a href="#" class="view-property-btn">View Property</a>
        </div>
        <div class="property-card hidden">
            <img src="home6.jpg" alt="Elegant Mansion">
            <h3>RS 30,00,00,000</h3>
            <p>Kathmandu</p>
            <a href="#" class="view-property-btn">View Property</a>
        </div>
    </div>

    <!-- View All button -->
    <div class="view-all-container">
        <button id="viewAllBtn">View All</button>
    </div>
</section>
<footer>
    <div class="footer-container">
        <div class="footer-info">
            <h3>Contact Us</h3>
            <p><strong>Phone:</strong> +977-1234567890</p>
            <p><strong>Email:</strong> info@realestate.com</p>
            <p><strong>Location:</strong> Kathmandu, Nepal</p>
        </div>
        <div class="footer-links">
            <h3>Quick Links</h3>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Properties</a></li>
                <li><a href="#">Gallery</a></li>
                <li><a href="#">Contact Us</a></li>
            </ul>
        </div>
    </div>
    <div class="footer-bottom">
        <p>&copy; 2025 Real Estate. All rights reserved.</p>
    </div>
</footer>

<script>
  const modal = document.getElementById("loginModal");
  const loginBtn = document.getElementById("loginBtn");
  const closeBtn = document.querySelector(".close");
  const loginForm = document.querySelector(".login-form");
  const passwordInput = document.getElementById("password");
  const showPasswordCheckbox = document.getElementById("showPassword");
  
  showPasswordCheckbox.addEventListener("change", function(){
  if(this.checked){
   passwordInput.type="text";
  }
  else{
   passwordInput.type="password";
  }
});   
  
  loginForm.addEventListener("submit", function(event){
   event.preventDefault();

   const email = document.getElementById("email").value;
   const password = document.getElementById("password").value;
    
   console.log("Email:", email);
   console.log("Password:", password);

   modal.classList.remove("active");
});

  loginBtn.addEventListener("click", function(event) {
    event.preventDefault(); // Prevent link navigation if it's an <a>
    modal.classList.add("active"); 
  });

  closeBtn.addEventListener("click", function() {
    modal.classList.remove("active");
  });

 
  window.addEventListener("click", function(event) {
    if (event.target === modal) {
      modal.classList.remove("active");
    }
  });
</script>
<script>
    document.getElementById("viewAllBtn").addEventListener("click", function() {
        const hiddenCards = document.querySelectorAll(".property-card.hidden");
        hiddenCards.forEach(card => card.classList.remove("hidden"));
        this.style.display = "none"; // Hide the button after clicking
    });
    </script>

</main>
</body>
</html>
