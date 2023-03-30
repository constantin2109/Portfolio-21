# portfolio-21...

Added 30 march 2023.


<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/all.min.css" />
    <link rel="stylesheet" href="css/style.css" />
    <title>My portfolio</title>
</head>

<body>
   
    <header>
        <!-- navbar start-->
        <nav>
            
            <a href="nasa.jpg" class="logo">
                <h2><span>R</span>ESUME</h2>
            </a>
            <ul>
              <li><a href="#">Home</a></li>  
                <li><a href="#">About</a></li>
                <li><a href="https://bootcamp.du.edu/blog/programming-skills/">Skills</a></li>
                <li><a href="#">Blog</a></li>
            </ul>
            <div class="social-icons">
                <a href="linkedin.com/in/constantin-bagrin-346b7717a"><i class="fa-brands fa-linkedin" style="font-size: 58px;"></i></a>
            </div>
        </nav> 
        <!--navbar close-->

        <!--start showcase-->
        <div class="content-wrapper">
        <div class="content-left">
        <p class="lead">Constantin Bagrin</p>
        <div class="txt-content">
            <div class="normal_txt"></div>
            <div class="normal_txt"> Front End Developer</div>
        </div>
        <p style="color:rgb(236, 204, 236); font-size: 1.5rem;text-decoration:underline rgb(69, 108, 10);" >
            <b style="color:#c31212; font-size: 2rem;">I'm </b>a motivated individual with a strong work ethic,
             experienced in military school and the construction industry,<span style="color:#c31212;"><b> transitioning to IT</b></span>. 
            I'm passionate about problem-solving, have excellent communication and interpersonal skills, and am a fast learner.
             I'm positive, reliable, and committed to taking on challenges.
             I'm confident I can make a valuable contribution to any organization. 
        </p>
        <button onclick="window.location.href = 'index2.html'" >Chat me</button>
        <button type="button">My CV</button>
        </div>
        <div class="content-right img-box" onclick="window.location.href='index2.html'">
            <img src="img.jpg" alt=""/>
          </div>
         
          
    </div>
    <!--close showcase-->

    <!-- skills start -->
    <div class="skills">
        <a href="https://github.com/constantin2109"> <h2>Skills</h2> </a>
        <div id="con"><i  class="fa-brands fa-html5 html" ></i></div>
        <div id="con1"><i class="fa-brands fa-css3-alt css3"></i></div>
        <div id="con2"><i class="fa-brands fa-js js" ></i></div>
        <div id="con3"><i class="fa-brands fa-react react"></i></div>
    </div>
    <!-- skills close-->
    </header>
    <script src="JS/script.js"></script>
   

    
</body>

</html>

——————————————————————————————

@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;800&display=swap');

:root {

    --primary-bg-color: #0c4d91;
    --secondary-bg-color: #999711;
    --txt-white: white;
    --primary-color: #1ed068;
    --box-shadow: 10px 8px #12f671;

}

}

* {
    /* background-image: url("nasa.jpg")*/
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    text-decoration: none;
    font-family: "Monserrat", sans-serif;
    overflow: hidden;
}


a {
    color: var(--txt-white);
}

header {
    color: var(--txt-white);
    background: var(--secondary-bg-color);
    font-size: 1.2rem;
    min-height: 100vh;
    width: 100%;
    display: none;
}

nav {
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 100%;
    background: var(--primary-bg-color);
    height: 80px;
}

nav ul {
    display: flex;
    list-style: none;
}

nav ul li {
    padding: 1.5rem 0.5rem;
    margin: 0 1.4rem;
    position: relative;
}

nav ul li a::after {
    content: "";
    position: absolute;
    left: 0;
    height: 3px;
    background: var(--primary-color);
    width: 0%;
    left: 0;
    top: 60px;
    transition: all 0.3s;
}

nav ul li a:hover:after {
    width: 100%;
}

.social-icons a {
    padding: 0 1rem;
    transition: all 0.4s;
}

.social-icons a:hover {
    color: var(--primary-color);


}

.lead {
    color: #286c18;
}

.logo {
    color: var(--primary-color);
    font-size: 1rem;
}






.logo span {
    font-size: 3rem;
}

/* Navbar close */

/* showcase start */
.content-wrapper {
    display: flex;
    align-items: center;
    justify-content: space-around;
    width: 100%;
    height: 84vh;
    padding: 0 10%;
}

.content-left {
    width: 70%;
}

.content-left .lead {
    font-size: 2rem;
    font-weight: 600;
}

.txt-content {
    display: flex;
    width: 100%;
}

.normal_txt {
    font-size: 3rem;
    width: 15%;
}

.change_txt {
    font-size: 3rem;
    color: var(--primary-color);
    font-weight: 600;
    position: relative;
}

/* Animation */
.txt-content.change_txt::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgb(0, 0, 0, 1);
    background: var(--secondary-bg-color);
    animation: animateTxt 4s steps(25) infinite;
}

/* Animation close */
.content-left p {
    font-size: 1rem;
    line-height: 2rem;
    margin: 1rem 0;
}

.content-left button {
    display: inline-block;
    background: transparent;
    border: 1px solid #fff;
    color: #fff;
    padding: 1rem 2rem;
    margin: 2rem 2rem 0 0;
    font-size: 1rem;
    cursor: pointer;
    border-radius: 02px;
    transition: all 0.5s;
}

.content-left button:hover {
    background: var(--primary-color);
    border: none;
    padding: 1rem 3rem;
}

.content-left button:active {
    transform: scale(0.95);
}

/* right-content start */
.content-right {
    width: 45%;
    box-shadow: var(--box-shadow);
    border-radius: 05px;
    background: #fff;
    transform: translateX(300%);

    animation: imgAnimate 5s forwards 2s;
}

.box {
    position: absolute;
    background-color: #61dafb;
    width: 300px;
    height: 300px;
    top: 50%;
    bottom: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    border: 10px solid #6F2DA8;
    margin: auto;
    text-align: center;
    border-radius: 0.5rem;
    overflow: hidden;
}

/*.p# {
    position: absolute;
    top: 45%;
    left: 50%;
    transform: translate(-50%, -50%);
}

/*p { 
    color:rgb(165, 136, 163);
    font-size: 5rem; 
}
    */




/*table {
                border-collapse: collapse;
                border-spacing: 0;
                width: 100%;
                border: 1px solid #ddd;
                text-align: center;
            }

            th, td {
                border: none;
                padding: 8px;
            }

            tr:nth-child(even){background-color: #f2f2f2}

            /* Animation */
@keyframes animateTable {
    from {
        background-color: #f9f9f9;
    }

    to {
        background-color: #ffffff;
    }
}

tr {
    animation: animateTable 1s ease-in-out infinite;
}




.content-right img {

    display: flex;
    text-align: center;
    min-height: 100%;
    width: 100%;
    border-radius: 05px;
    animation: myAnimation 5s linear;
}


/* right-content close */
/* Skills start */
.skills {
    display: flex;
    justify-content: space-around;
    align-items: center;
    background: var(--primary-bg-color);
    color: #fff;
    width: 100%;
    padding: 0 01%;

}

.skills h2 {
    font-size: 2.8rem;
    padding: 0.5rem 0;
    color: var(--primary-color);

}

.skills i {
    font-size: 3rem;
    cursor: pointer;
}

.skills .css3 {
    color: #1875b8;
}

.skills .html {
    color: #e44f26;
}

.skills .js {
    color: #ffd700;
}

.skills .react {
    color: #61dafb;
}

/* Skills close */
/* Animation start */
@keyframes imgAnimate {
    to {
        transform: translateX(0);
        transform: skew(-2deg);

    }
}


@keyframes animateTxt {
    3% {
        left: 0;
    }

    30% {
        left: 100%;
    }

    80% {
        left: 100%;
    }

    100% {
        left: 0;
    }
}

/* Animation close */
/* shocase close */
@media screen and ( max-width: 600px)
{
   h1{
    font-size: 36px;
    line-height: 50px;
   }
}
@media (min-width: 768px) {
    p {
        font-size: 1.5rem;
    }
}

@media (max-width: 768px) {
    p {
        font-size: 1.2rem;
    }
}
  
——————————————————————————————————
   Index 2 

    <html> 
  <head> 
    <title>Page2</title> 
    <link rel="stylesheet" href="css/style2.css" />
    <script src="https://apps.elfsight.com/p/platform.js" defer></script>
   <div class="elfsight-app-950ab59e-1a30-4f13-8bbf-e13130dfafa2" ></div>
  </head> 
  
  <body> 
  
    
    
    
  </body> 
</html> 
      

———————————————————————————————————

