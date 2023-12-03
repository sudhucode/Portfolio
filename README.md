<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sudhanshu's Portfolio</title>
    <link rel="stylesheet" href="style.css">
    <link rel="shortcut icon" href="photo/round-photo-logo.png" type="image/x-icon">
    <script src="https://kit.fontawesome.com/c58add7555.js" crossorigin="anonymous"></script>
</head>
  <style>
    *{
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
    box-sizing: border-box;
}
html{
    scroll-behavior: smooth;
}
body{
    background-color: #080808;
    color: white;
}

#header{
    width: 100%;
    height: 100vh;
    background-image: url(photo/background\ image.jpeg.jpg);
    background-size: cover;
    background-position: center;
}
.container{
    padding: 10px 10%;
}
nav{
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
}

.logo{
    width: 140px;

}
.container2{
    margin-left: 4px;
    align-items: center;}
span{
    color: #4070F4;
}
nav ul li{
    display: inline-block;
    list-style: none;
    margin: 10px 20px;
}

nav ul li a{
    color: white;
    text-decoration: none;
    font-size: 18px;
    position: relative;
}
nav ul li a::after{
    content: '';
    width: 0;
    height: 3px;
    background: #ff004f;
    position: absolute;
    left: 0;
    bottom: -6px;
    transition: 0.5s;
}
nav ul li a:hover::after{
    width: 100%;
}
.header-text{
    margin-top: 20%;
    font-size: 30px;
}
.header-text h1{
    font-size: 60px;
    margin-top: 20px;
}
.header-text h1 span{
    color: #ff004f;
}
/*------about-----*/
#about{
    padding: 80px 0;
    color: ababab;
}
.row{
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}
.about-col-1{
    flex-basis: 35%;

}
.about-col-1 img{
    width: 100%;
    border-radius: 15px;
}
.about-col-2{
    flex-basis: 60%;
}
.sub-titlle{
    font-size: 60px;
    font-weight: 600;
    color: white;
}
.tab-titles{
    display: flex;
    margin: 20px 0 40px;
}

.tab-links{
    margin-right: 50px;
    font-size: 18px;
    font-weight: 500;
    cursor: pointer;
    position: relative
}

.tab-links::after{
    content: '';
    width: 0;
    height: 3px;
    background: #ff004f;
    position: absolute;
    left: 0;
    bottom: -8px;
    transition: 0.5s;   
}
.tab-links.active-link::after{
    width: 50%;
}

.tab-contents ul li{
    list-style: none;
    margin: 10px 0;
}

.tab-contents ul li span{
    color: #b54769;
    font-size: 14px;
}
.tab-contents{
    display: none;
}
.tab-contents.active-tab{
    display: block;
}

/*----------------services------------*/
#services{
    padding: 30px 0;
}
.services-list{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 40px;
    margin-top: 50px;
}
.services-list div{
    background: #262626;
    padding: 40px;
    font-size: 13px;
    font-weight: 300;
    border-radius: 10px;
    transition: background 0.5s, transform 0.5s;
}
.services-list div i{
    font-size: 50px;
    margin-bottom: 30px;
}
.services-list div h2{
    font-size: 30px;
    font-weight: 500;
    margin-bottom: 15px;
}
.services-list div a{
    text-decoration: none;
    color: #fff;
    font-size: 12px;
    margin-top: 20px;
    display: inline-block;
}
.services-list div:hover{
    background: #ff004f;
    transform: translateY(-10px);
}
/*------------Protfolio-----------*/
#protfolio{
    padding: 50px 0;

}
.work-list{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 40px;
    margin-top: 50px;
}
.work{
    border-radius: 10px;
    position: relative;
    overflow: hidden;
}
.work img{
    width: 100%;
    border-radius: 10px;
    display: block;
    transition: transform 0.5s;
}
.layer{
    width: 100%;
    height: 0;
    background: linear-gradient(rgba(0,0,0,0.6), #ff004f);
    border-radius: 10px;
    position: absolute;
    left: 0;
    bottom: 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 0 40px;
    text-align: center;
    font-size: 14px;
    transition: height 0.5s;
}
.layer h3{
    font-weight: 500;
    margin-bottom: 20px;
}
.layer a{
    margin-top: 20px;
    color: #ff004f;
    text-decoration: none;
    font-size: 18px;
    line-height: 60px;
    background: white;
    width: 60px;
    height: 60px;
    border-radius: 50px;
    text-align: center;
}
.work:hover img{
    transform: scale(1.1);
}
.work:hover .layer{
    height: 100%;
}
.btn{
    display: block;
    margin: 50px auto;
    width: fit-content;
    border: 1px solid #ff004f;
    padding: 14px 50px;
    border-radius: 6px;
    text-decoration: none;
    color: white;
    transition: background 0.5s;
    box-shadow: 0 0 5px #ff004f, 0 0 25px #ff004f;
}
.btn:hover{
    background: #ff004f;
    box-shadow: 0 0 5px #ff004f, 0 0 25px #ff004f, 0 0 50px #ff004f, 0 0 100px #ff004f;
}
/*--------------contact---------*/
.contact-left{
    flex-basis: 35%;
}
.contact-right{
    flex-basis: 60%;
}
.contact-left p{
    margin-top: 30px;
}
.contact-left p i{
    color: #ff004f;
    margin-right: 15px;
    font-size: 25px;
}
.social-icon{
    margin-top: 30px;
}
.social-icon a{
    text-decoration: none;
    font-size: 30px;
    margin-right: 15px;
    color: #ababab;
    display: inline-block;
    transition: transform 0.5s;
}
.social-icon a:hover{
    color: #ff004f;
    transform: translateY(-5px);
}
.btn2{
    display: inline-block;
    background: #ff004f;
    margin: 50px auto;
    width: fit-content;
    border: 1px solid #ff004f;
    padding: 14px 50px;
    border-radius: 6px;
    text-decoration: none;
    color: white;
}.contact-right{
    width: 100%;
}
form input, form textarea{
    width: 100%;
    border: 0;
    outline: none;
    background: #262626;
    padding: 15px;
    margin: 15px 0;
    color: #fff;
    font-size: 18px;
    border-radius: 6px;
}
form .btn2{
    padding: 14px 60px;
    font-size: 18px;
    margin-top: 20px;
    cursor: pointer;
}
.copyright{
    width: 100%;
    text-align: center;
    padding: 25px 0;
    background: #262626;
    font-weight: 300;
    margin-top: 20px;
}
.copyright i{
    color: #ff004f;
}
/*------------css for small screens----------*/
nav .fa-solid{
    display: none;
}
@media only screen and (max-width: 600px){
    #header{
        background-image: url(photo/backgroundforphone.jpg);
    }
    .header-text{
        margin-top: 100%;
        font-size: 16px;
    }
    .header-text h1{
        font-size: 30px;
    }
    nav .fa-solid{
        display: block;
        font-size: 25px;
    }
    nav ul{
        background: #ff004f;
        position: fixed;
        top: 0;
        right: -200px;
        width: 200px;
        height: 100vh;
        padding-top: 50px;
        z-index: 2;
        transition: right 0.5s;
    }
    nav ul li{
        display: block;
        margin: 25px;
    }
    nav ul .fa-solid{
        position: absolute;
        top: 25px;
        left: 25px;
        cursor: pointer;
    }
    .sub-titlle{
        font-family: 40px;
    }
    .about-col-1, .about-col-2{
        flex-basis: 100%;
    }
    .about-col-1{
        margin-bottom: 30px;
    }
    .about-col-2{
        font-size: 14px;
    }
    .tab-links{
        font-size: 16px;
        margin-right: 20px;
    }
    .contact-left, .contact-right{
        flex-basis: 100%;
    }
    .copyright{
        font-size: 14px;
    }
}
#msg{
    color: #61b752;
    margin-top: -40px;
    display: block;
}

#preloader{
    background: #1b1d21 url(photo/loader.gif) no-repeat center center;
    background-size: 30%;
    height: 100vh;
    width: 100%;
    position: fixed;
    z-index: 100;
}
  </style>
<body>
    <div id="preloader"></div>
    <div id="header">
        <div class="container">
            <nav>
                <img src="photo/logo.jpg" class="logo">
                <ul id="sidemenu">
                    <li><a href="#header">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#protfolio">Portfolio</a></li>
                    <li><a href="#contact">Contact</a></li>
                    <i class="fa-solid fa-x" onclick="closemenu()"></i>
                </ul>
                <i class="fa-solid fa-bars" onclick="openmenu()"></i>
            </nav>
            <div class="header-text">
                <p>UI/UX Designer</p>
                <h1>Hi, I'm <span>§µÐhåñ§hµ</span><br>From Bihar </h1>
            </div>
        <div class="container2">
            <h2>I'm a <span class="auto-type"></span></h2>
        </div>

            <script src="https://unpkg.com/typed.js@2.1.0/dist/typed.umd.js"></script>

            <script>
                var typed = new Typed(".auto-type", {
                    strings: ["YouTuber", "Coder", "Blogger", "Freelancer"],
                    typeSpeed: 80,
                    backSpeed: 80,
                    loop: true
                })
            </script>


        </div>
    </div>
   <!---------about------->
    <div id="about">
        <div class="container">
            <div class="row">
                <div class="about-col-1">
                    <img src="/photo/user1.jpg">
                </div>
                <div class="about-col-2">
                    <h1 class="sub-title">About Me</h1>
                    <p>I'm a talented and passionate web developer and graphic designer. I love creating visually appealing websites and designing stunning graphics. With my skills in HTML, CSS, JavaScript, and Photoshop, I can bring your ideas to life. Let's collaborate and make something amazing together!</p>
                    <div class="tab-titles">
                        <p class="tab-links active-link" onclick="opentab('skills')">Skills</p>
                        <p class="tab-links" onclick="opentab('experience')">Experience</p>
                        <p class="tab-links"onclick="opentab('education')">Education</p>
                    </div>
                    <div class="tab-contents active-tab" id="skills">
                        <ul>
                            <li><span>UI/UX</span><br>Designing Web/App interfaces</li>
                            <li><span>Web devlopment</span><br>Web app Development</li>
                            <li><span>App Devlopment</span><br>Building Android GAMES</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="experience">
                        <ul>
                            <li><span>2023 - Current</span><br>Studiying in 12th class</li>
                            <li><span>2021 - 2022</span><br>10th passed form state board</li>
                            <li><span>2019 - 2021</span><br>Studied from High School</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="education">
                        <ul>
                            <li><span>2022 - current</span><br>Learning Web devloping from YouTube</li>
                            <li><span>2020 - 2022</span><br>Learned Graphics Designing from YouTube</li>
                            <li><span>2017 - 2020</span><br>Learned repairing Electrical Product from YouTube</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
<!------------Services----------->
<div id="services">
    <div class="container">
        <h1 class="sub-title">My Services</h1>
        <div class="services-list">
            <div>
                <i class="fa-solid fa-code"></i>
                <h2>Web Design</h2>
                <p> Our team of talented designers can create a stunning website just for you. Let's make your online presence stand out!</p>
                <a href="#">Learn more</a>
            </div>
             <div>
                <i class="fa-solid fa-crop-simple"></i>
                <h2>UI/UX Design</h2>
                <p>  Just let me know your requirements and preferences, and I'll create an amazing design for you!</p>
                <a href="#">Learn more</a>
            </div>
            <div>
                <i class="fa-brands fa-app-store"></i>
                <h2>App Design</h2>
                    <p> Do you have any specific requirements in mind? Let me know, and I'll assist you with it</p>
                    <a href="#">Learn more</a>
            </div>
           
        </div>
    </div>
</div>
<!-----------Protfolio---------->
<div id="protfolio">
    <div class="container">
        <h1 class="sub-title">My Work</h1>
        <div class="work-list">
            <div class="work">
                <img src="photo/work-1.png">
                <div class="layer">
                    <h3>App Devloping</h3>
                    <p>I can make social media Apps using computer software <br> Like Xamarin, BuildFire etc..</p>
                        <a href="#"><i class="fa-solid fa-up-right-from-square"></i></a>
                </div>
            </div>
            <div class="work">
                <img src="photo/work-2.png">
                <div class="layer">
                    <h3>Web Devloping</h3>
                    <p>I can make OSm Websites using these launguages <br>HTML, CSS, JAVASCERIPT etc.</br></p>
                        <a href="#"><i class="fa-solid fa-up-right-from-square"></i></a>
                </div>
            </div>
            <div class="work">
                <img src="photo/work-3.png">
                <div class="layer">
                    <h3>Graphics Designing</h3>
                    <p>I can make YouTube thumbnail, Poster, Visiting card etc...</p>
                        <a href="#"><i class="fa-solid fa-up-right-from-square"></i></a>
                </div>
            </div>
        </div>
        <a href="#" class="btn">See more</a>
    </div>
</div>

<!------contact------->
<div id="contact">
    <div class="container">
        <div class="row">
            <div class="contact-left">
                <h1 class="sub-title">Contact Me</h1>
                <p><i class="fa-solid fa-paper-plane"></i> sudhuraj@123gmail.com</p>
                <p><i class="fa-solid fa-phone"></i> +91 91224 95060</p>
                <div class="social-icon">
                    <a href="https://www.facebook.com/profile.php?id=100036861284080"><i class="fa-brands fa-facebook"></i></a>
                    <a href="https://www.instagram.com/ig__sudhanshu__/"><i class="fa-brands fa-instagram"></i></a>
                    <a href="https://www.youtube.com/@sudhanshutech20"><i class="fa-brands fa-youtube"></i></a>
                    <a href="https://twitter.com/ig__sudhanshu__"><i class="fa-brands fa-twitter"></i></a>

                </div>
                <a href="photo/my-cv.pdf" download class="btn2">Download CV</a>
            </div>
            <div class="contact-right">
                <form name="submit-to-google-sheet">
                    <input type="text" name="Name" placeholder="Yourname" required>
                    <input type="email" name="Email" placeholder="Your Email" required>
                    <textarea name="Message" rows="6" placeholder="Your Message"></textarea>
                    <button type="submit" class="btn2">Submit</button>
                </form>
                <span id="msg"></span>
            </div>
        </div>
    </div>
    <div class="copyright">
        <p>Copyright © §µÐhµ. Made with <i class="fa-solid fa-heart"></i> Sudhanshu Tech</p>
    </div>
</div>


    <script>
        var tablinks = document.getElementsByClassName("tab-links")
        var tabcontents = document.getElementsByClassName("tab-contents")
        function opentab(tabname){
            for(tablink of tablinks){
                tablink.classList.remove("active-link");
            }
            for(tabcontent of tabcontents){
                tabcontent.classList.remove("active-tab");
            }
            event.currentTarget.classList.add("active-link");
            document.getElementById(tabname).classList.add("active-tab");
        }

    </script>
    <script>
        var sidemenu = document.getElementById("sidemenu")
        function openmenu(){
            sidemenu.style.right = "0"
        }
        function closemenu(){
            sidemenu.style.right = "-200px"
        }
    </script>
    <script>
        const scriptURL = 'https://script.google.com/macros/s/AKfycbzf0rzuzVu5lzZ3tuEYYrVQd3MrJeQSvgJs33rek-XIDm75p8c8uba6ZZWWoMCoac2d/exec'
        const form = document.forms['submit-to-google-sheet']
        const msg = document.getElementById("msg")
      
        form.addEventListener('submit', e => {
          e.preventDefault()
          fetch(scriptURL, { method: 'POST', body: new FormData(form)})
            .then(response => {
                msg.innerHTML = "Message sent successfully"
                setTimeout(function(){
                    msg.innerHTML = ""
                },5000)
                form.reset()
            })
            .catch(error => console.error('Error!', error.message))
        })
      </script>

      <script>
        var loader = document.getElementById("preloader");

        window.addEventListener("load", function(){
            loader.style.display = "none";
        })

      </script>
</body>
</html>
