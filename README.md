<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>W3.CSS Template</title>
    <link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Montserrat">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <style>
        body, h1, h2, h3, h4, h5, h6 {font-family: "Montserrat", sans-serif}
        .w3-row-padding img {margin-bottom: 12px}
        .w3-sidebar {width: 120px;background: #222;}
        #main {margin-left: 120px}
        @media only screen and (max-width: 600px) {#main {margin-left: 0}}
        img {max-width: 100%; height: auto; display: block;}
    </style>
</head>
<body class="w3-black">

<!-- Icon Bar (Sidebar - hidden on small screens) -->
<nav class="w3-sidebar w3-bar-block w3-small w3-hide-small w3-center">
  <!-- Avatar image in top left corner -->
  <img src="https://lh3.googleusercontent.com/pw/AP1GczP8Yaix7UXAEl2a9lj280nYUXnD9IC04-3JSHTRqePfAV7PX7q7KEBxi8ZCkXn55BoXTsB70_AeMtzSLLje67TUuZWp5ZqIwS_RR6d7Im--JEZYNFo=w600-h315-p-k" alt="Avatar" style="width:100%">
  <a href="#" class="w3-bar-item w3-button w3-padding-large w3-black">
    <i class="fa fa-home w3-xxlarge"></i>
    <p>HOME</p>
  </a>
  <a href="#about" class="w3-bar-item w3-button w3-padding-large w3-hover-black">
    <i class="fa fa-user w3-xxlarge"></i>
    <p>ABOUT</p>
  </a>
  <a href="#photos" class="w3-bar-item w3-button w3-padding-large w3-hover-black">
    <i class="fa fa-eye w3-xxlarge"></i>
    <p>PHOTOS</p>
  </a>
  <a href="#contact" class="w3-bar-item w3-button w3-padding-large w3-hover-black">
    <i class="fa fa-envelope w3-xxlarge"></i>
    <p>CONTACT</p>
  </a>
</nav>

<!-- Navbar on small screens (Hidden on medium and large screens) -->
<div class="w3-top w3-hide-large w3-hide-medium" id="myNavbar">
  <div class="w3-bar w3-black w3-opacity w3-hover-opacity-off w3-center w3-small">
    <a href="#" class="w3-bar-item w3-button" style="width:25% !important">HOME</a>
    <a href="#about" class="w3-bar-item w3-button" style="width:25% !important">ABOUT</a>
    <a href="#photos" class="w3-bar-item w3-button" style="width:25% !important">PHOTOS</a>
    <a href="#contact" class="w3-bar-item w3-button" style="width:25% !important">CONTACT</a>
  </div>
</div>

<!-- Page Content -->
<div class="w3-padding-large" id="main">
  <!-- Header/Home -->
  <header class="w3-container w3-padding-32 w3-center w3-black" id="home">
    <h1 class="w3-jumbo"><span class="w3-hide-small">I'm</span> Israel Kukoyi.</h1>
    <p>Cashier</p>
    <img src="https://lh3.googleusercontent.com/pw/AP1GczP8Yaix7UXAEl2a9lj280nYUXnD9IC04-3JSHTRqePfAV7PX7q7KEBxi8ZCkXn55BoXTsB70_AeMtzSLLje67TUuZWp5ZqIwS_RR6d7Im--JEZYNFo=w600-h315-p-k" alt="boy" class="w3-image">
  </header>

  <!-- About Section -->
  <div class="w3-content w3-justify w3-text-grey w3-padding-64" id="about">
    <h2 class="w3-text-light-grey">My Name</h2>
    <hr style="width:200px" class="w3-opacity">
    <p> My name is Israel Kukoyi. I am a Nigerian-Canadian first-generation immigrant and a second-year Information Technology major at York University. I am multilingual, fluent in French, English, and Yoruba, with several months of learning Spanish on Duolingo. I have hands-on experience in coding and website creation/design, and I have volunteered at my local church as an audio and visual engineer. Additionally, I have work experience as a cashier at McDonald's and Tim Hortons, where I developed strong customer service and cash handling skills.

    During my studies, I have worked on several notable projects, including developing a responsive website for a local business and creating a basic game using Python. These experiences have honed my technical skills and sparked my passion for software development.
    Outside of work and academics, I am passionate about writing, reading, gaming, and software. I enjoy creating scripts and codes for future game ideas during my free time. Volunteering at my local church has taught me valuable lessons in teamwork and community service.

    Currently, I am unemployed, but I am actively seeking opportunities to gain more experience in the IT field. Looking ahead, I aim to complete my education and pursue a career in software development or IT management. My long-term goal is to become a lead developer in a tech company, contributing to innovative projects and making a significant impact in the industry. I am eager to continue learning and growing, both personally and professionally, and I am excited about the future opportunities that lie ahead.
    </p>
    <h3 class="w3-padding-16 w3-text-light-grey">My Skills</h3>
    <p class="w3-wide">Customer Service</p>
    <div class="w3-white">
      <div class="w3-dark-grey" style="height:28px;width:95%"></div>
    </div>
    <p class="w3-wide">Web Creation and Design</p>
    <div class="w3-white">
      <div class="w3-dark-grey" style="height:28px;width:85%"></div>
    </div>
    <p class="w3-wide">Book Balancing</p>
    <div class="w3-white">
      <div class="w3-dark-grey" style="height:28px;width:85%"></div>
    </div>
    <p class="w3-wide">Food handling and safety</p>
    <div class="w3-white">
      <div class="w3-dark-grey" style="height:28px;width:80%"></div>
    </div><br>
    
    <div class="w3-row w3-center w3-padding-16 w3-section w3-light-grey">
      <div class="w3-quarter w3-section">
        <span class="w3-xlarge">3+</span><br>
        Paid Jobs
      </div>
      <div class="w3-quarter w3-section">
        <span class="w3-xlarge">10+</span><br>
        Projects Done
      </div>
      <div class="w3-quarter w3-section">
        <span class="w3-xlarge">190+</span><br>
        Happy Customers
      </div>
      <div class="w3-quarter w3-section">
        <span class="w3-xlarge">600+</span><br>
        Volunteer Days 
      </div>
    </div>

    <button class="w3-button w3-light-grey w3-padding-large w3-section">
      <i class="fa fa-download"></i> Download Resume
    </button>
    
  <!-- Portfolio Section -->
  <div class="w3-padding-64 w3-content" id="work-history">
    <h2 class="w3-text-light-grey">Work History</h2>
    <hr style
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Israel Kukoyi - Portfolio</title>
    <link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Montserrat">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <style>
        body,
        h1,
        h2,
        h3,
        h4,
        h5,
        h6 {
            font-family: "Montserrat", sans-serif;
        }

        .w3-row-padding img {
            margin-bottom: 12px;
        }

        .w3-sidebar {
            width: 120px;
            background: #222;
        }

        #main {
            margin-left: 120px;
        }

        @media only screen and (max-width: 600px) {
            #main {
                margin-left: 0;
            }
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
        }
    </style>
</head>

<body class="w3-black">

    <!-- Icon Bar (Sidebar - hidden on small screens) -->
    <nav class="w3-sidebar w3-bar-block w3-small w3-hide-small w3-center">
        <!-- Avatar image in top left corner -->
        <img src="https://lh3.googleusercontent.com/pw/AP1GczP8Yaix7UXAEl2a9lj280nYUXnD9IC04-3JSHTRqePfAV7PX7q7KEBxi8ZCkXn55BoXTsB70_AeMtzSLLje67TUuZWp5ZqIwS_RR6d7Im--JEZYNFo=w600-h315-p-k"
            alt="Avatar" style="width:100%">
        <a href="#" class="w3-bar-item w3-button w3-padding-large w3-black">
            <i class="fa fa-home w3-xxlarge"></i>
            <p>HOME</p>
        </a>
        <a href="#about" class="w3-bar-item w3-button w3-padding-large w3-hover-black">
            <i class="fa fa-user w3-xxlarge"></i>
            <p>ABOUT</p>
        </a>
        <a href="#photos" class="w3-bar-item w3-button w3-padding-large w3-hover-black">
            <i class="fa fa-eye w3-xxlarge"></i>
            <p>PHOTOS</p>
        </a>
        <a href="#contact" class="w3-bar-item w3-button w3-padding-large w3-hover-black">
            <i class="fa fa-envelope w3-xxlarge"></i>
            <p>CONTACT</p>
        </a>
    </nav>

    <!-- Navbar on small screens (Hidden on medium and large screens) -->
    <div class="w3-top w3-hide-large w3-hide-medium" id="myNavbar">
        <div class="w3-bar w3-black w3-opacity w3-hover-opacity-off w3-center w3-small">
            <a href="#" class="w3-bar-item w3-button" style="width:25% !important">HOME</a>
            <a href="#about" class="w3-bar-item w3-button" style="width:25% !important">ABOUT</a>
            <a href="#photos" class="w3-bar-item w3-button" style="width:25% !important">PHOTOS</a>
            <a href="#contact" class="w3-bar-item w3-button" style="width:25% !important">CONTACT</a>
        </div>
    </div>

    <!-- Page Content -->
    <div class="w3-padding-large" id="main">
        <!-- Header/Home -->
        <header class="w3-container w3-padding-32 w3-center w3-black" id="home">
            <h1 class="w3-jumbo"><span class="w3-hide-small">I'm</span> Israel Kukoyi.</h1>
            <p>Cashier</p>
            <img src="https://lh3.googleusercontent.com/pw/AP1GczP8Yaix7UXAEl2a9lj280nYUXnD9IC04-3JSHTRqePfAV7PX7q7KEBxi8ZCkXn55BoXTsB70_AeMtzSLLje67TUuZWp5ZqIwS_RR6d7Im--JEZYNFo=w600-h315-p-k"
                alt="boy" class="w3-image">
        </header>

        <!-- About Section -->
        <div class="w3-content w3-justify w3-text-grey w3-padding-64" id="about">
            <h2 class="w3-text-light-grey">My Name</h2>
            <hr style="width:200px" class="w3-opacity">
            <p>My name is Israel Kukoyi... (Rest of your biography text here)</p>

            <h3 class="w3-padding-16 w3-text-light-grey">My Skills</h3>
            <p class="w3-wide">Customer Service</p>
            <div class="w3-white">
                <div class="w3-dark-grey" style="height:28px;width:95%"></div>
            </div>
            <p class="w3-wide">Web Creation and Design</p>
            <div class="w3-white">
                <div class="w3-dark-grey" style="height:28px;width:85%"></div>
            </div>
            <p class="w3-wide">Book Balancing</p>
            <div class="w3-white">
                <div class="w3-dark-grey" style="height:28px;width:85%"></div>
            </div>
            <p class="w3-wide">Food handling and safety</p>
            <div class="w3-white">
                <div class="w3-dark-grey" style="height:28px;width:80%"></div>
            </div><br>

            <!-- Stats Section -->
            <div class="w3-row w3-center w3-padding-16 w3-section w3-light-grey">
                <div class="w3-quarter w3-section">
                    <span class="w3-xlarge">3+</span><br>
                    Paid Jobs
                </div>
                <div class="w3-quarter w3-section">
                    <span class="w3-xlarge">10+</span><br>
                    Projects Done
                </div>
                <div class="w3-quarter w3-section">
                    <span class="w3-xlarge">190+</span><br>
                    Happy Customers
                </div>
                <div class="w3-quarter w3-section">
                    <span class="w3-xlarge">600+</span><br>
                    Volunteer Days
                </div>
            </div>

            <button class="w3-button w3-light-grey w3-padding-large w3-section">
                <i class="fa fa-download"></i> Download Resume
            </button>
        </div>

        <!-- Portfolio Section -->
        <div class="w3-padding-64 w3-content" id="work-history">
            <h2 class="w3-text-light-grey">Work History</h2>
            <hr style="width:200px" class="w3-opacity">
            <!-- Continue your content -->
        </div>

    </div>

</body>

</html>
