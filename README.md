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
            <li class="nav-item"><a href="#" class="nav-link">About</a></li>
            <li class="nav-item"><a href="#" class="nav-link">Properties</a></li>
            <li class="nav-item"><a href="#" class="nav-link">Buy/Rent</a></li>
            <li class="nav-item"><a href="#" class="nav-link">Contact Us</a></li>
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
<script>
  const modal = document.getElementById("loginModal");
  const loginBtn = document.getElementById("loginBtn");
  const closeBtn = document.querySelector(".close");
  const loginForm = document.querySelector(".login-form");
  const passwordInput = document.getElementById("password");
  const showPasswordCheckbox = document.getElementById("showPassword");
  
  showPasswordCheckbox.addEventListener("change", function(){
  if(this.check){
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

</main>
</body>
</html>
