# Task3_Tourisam

<!DOCTYPE html>
<html>
    <head>
        <style>
            *{box-sizing:border-box}


.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

.Containers {
  display: none;
}

/* Code for the forward & Back buttons */
.Back, .forward {
  cursor: pointer;
  position: absolute;
  top: 48%;
  width: auto;
  margin-top: -23px;
  padding: 17px;
  color: grey;
  font-weight: bold;
  font-size: 19px;
  transition: 0.4s ease;
  border-radius: 0 5px 5px 0;
  user-select: none;
}


.forward {
  right: 0;
  border-radius: 4px 0 0 4px;
}

.Back:hover, .forward:hover {
  background-color: rgba(0,0,0,0.8);
}


.Info {
  color: #e3e3e3;
  font-size: 16px;
  padding: 10px 14px;
  position: absolute;
  bottom: 10px;
  width: 100%;
  text-align: center;
}

/* Image numbering  */
.MessageInfo {
  color: #f2f2f3;
  font-size: 14px;
  padding: 10px 14px;
  position: absolute;
  top: 0;
}


.dots {
  cursor: pointer;
  height: 16px;
  width: 16px;
  margin: 0 3px;
  background-color: #acc;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.5s ease;
}

.enable, .dots:hover {
  background-color: #717161;
}


.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1.4s;
  animation-name: fade;
  animation-duration: 1.4s;
}

@-webkit-keyframes fade {
  from {opacity: .5}
  to {opacity: 2}
}

@keyframes fade {
  from {opacity: .5}
  to {opacity: 2}
}
        </style>
        
        <title>Tourism</title>
    <script>
       var slidePosition = 0;
SlideShow(slidePosition);

// forward/Back controls
function plusSlides(n) {
  SlideShow(slidePosition += n);
}

function plusSlides1(n) {
  SlideShow(slidePosition += n);
}

//  images controls
function currentSlide(n) {
  SlideShow(slidePosition = n);
}

function SlideShow(n) {
  var i;
  var slides = document.getElementsByClassName("Containers");
  var circles = document.getElementsByClassName("dots");
  if (n > slides.length) {slidePosition = 1}
  if (n < 1) {slidePosition = slides.length}
  for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";
  }
  for (i = 0; i < circles.length; i++) {
      circles[i].className = circles[i].className.replace(" enable", "");
  }
  slides[slidePosition-1].style.display = "block";
  circles[slidePosition-1].className += " enable";
} 

    </script>

    <link href="Tourism_css.css" rel="stylesheet" type="text/css">
    </head>

    <header>
        <ul id= "left-nav">
            <li href="touri.jpg">Logo</li>
        </ul>

        <ul id= "right-nav">
            <li href="">Destinations</li>
        </ul>

        <ul id= "right-nav">
            <li href="">Contact us</li>
        </ul>
    </header>

    <style>
        /* Add some padding on document's body to prevent the content
        to go underneath the header and footer */
        body{        
            padding-top: 60px;
            padding-bottom: 40px;
        }
        .fixed-header, .fixed-footer{
            width: 100%;
            position: fixed;        
            background: #333;
            padding: 10px 0;
            color: #fff;
        }
        .fixed-header{
            top: 0;
        }
        .fixed-footer{
            bottom: 0;
        }
        .container{
            width: 80%;
            margin: 0 auto; /* Center the DIV horizontally */
        }
        nav a{
            color: #fff;
            text-decoration: none;
            padding: 7px 25px;
            display: inline-block;
        }
    </style>
    
    <body>
        <div class="slideshow-container fade">

            <!-- Full images with numbers and message Info -->
            <div class="Containers" style="display: block;">
                <div class="MessageInfo">1 / 4</div>
                <img src="tour.jpg" style="width:100%">
                <div class="Info">First caption</div>
              </div>

            <div class="Containers" style="display: block;">
              <div class="MessageInfo">2 / 4</div>
              <img src="kankria.jpg" style="width:100%">
              <div class="Info">second caption</div>
            </div>
          
            <div class="Containers">
              <div class="MessageInfo">3 / 4</div>
              <img src="city.jpg" style="width:100%">
              <div class="Info">Third Caption</div>
            </div>
          
            <div class="Containers">
              <div class="MessageInfo">4 / 4</div>
              <img src="aashram.jpg" style="width:100%">
              <div class="Info">Fourth Caption</div>
            </div>
          
            <!-- Back and forward buttons -->
            <a class="Back" onclick="plusSlides(-1)">&#10094;</a>
            <a class="forward" onclick="plusSlides(1)">&#10095;</a>
          </div>
          <br>
          
          <!-- The circles/dots -->
          <div style="text-align:center">
            <span class="dots" onclick="currentSlide(1)"></span>
            <span class="dots" onclick="currentSlide(2)"></span>
            <span class="dots" onclick="currentSlide(3)"></span>
            <span class="dots" onclick="currentSlide(4)"></span>
          </div>

       

        <header>
            <h1> Kankariya lake</h1>
             
        <img src="kankria.jpg" alt="View of Kankaria lake"> 
        </header>
        <article>
            <p>Kankaria Lake is the second largest lake in Ahmedabad, Gujarat, India. It is located in the south-eastern part of the city, in the Maninagar area. 
            It was completed in 1451 during the reign of Sultan Qutb-ud-Din Ahmad Shah II though its origin is placed in the Chaulukya period sometimes. 
            A lakefront is developed around it, which has many public attractions such as a zoo, toy train, kids city, tethered balloon ride, water rides, water park, food stalls, and entertainment facilities. 
            The lakefront was revamped in 2007–2008. Kankaria Carnival is a week-long festival held here in the last week of December.</p>
            
            <p>Many cultural, art, and social activities are organised during the carnival. Kankaria Carnival is an annual week-long cultural festival organised in last week of December since 2008. 
            The festival include art, dance and music performances, social awareness programmes, games and activities for children,</p>

            <p><a href="https://en.wikipedia.org/wiki/Kankaria_Lake" target="_blank">Read more</a>to find out more details about kankria</p>
        </article>

        <header>
            <h1> Science City</h1>
            <div class="slideshow-container fade">

                
            <img src="city.jpg" alt="View of Science city"> 
        </header>
        <article>
            <p>Gujarat Science City is a science education and entertainment centre located in Ahmedabad, Gujarat, India. 
                Opened in 2002, it has an IMAX 3D theatre; exhibitions on science, space, energy, life sciences, plants, nature and robotics; an aquarium, an aviary and a butterfly park; as well as other facilities.</p>
            
            <p>The park spread over an area of 9000 sqm is dedicated to life sciences. It has exhibits on river system and evolution. 
                It also has outdoor exhibition on aromatic, medicinal and economic plants as well as ornamental plants. 
                There is a Cactus, Succulent and Bonsai Corner; Butterfly House; aviary and tissue culture lab</p>

            <p><a href="https://en.wikipedia.org/wiki/Gujarat_Science_City" target="_blank">Read more</a>to find out more details about Science city</p>
        </article>

        <header>
            <h1> Gnadhi Aashram</h1>
            <img src="aashram.jpg" alt="Sabarmati aashram"> 
        </header>
        <article>
            <p>Sabarmati Ashram (also known as Gandhi Ashram) is located in the Sabarmati suburb of Ahmedabad, Gujarat, adjoining the Ashram Road, on the banks of the River Sabarmati, 4 miles (6.4 km) from the town hall. 
                This was one of the many residences of Mahatma Gandhi who lived at Sabarmati (Gujarat) and Sevagram (Wardha, Maharashtra) when he was not travelling across India or in prison.
                 He lived in Sabarmati or Wardha for a total of twelve years with his wife Kasturba Gandhi and followers, including Vinoba Bhave. 
                 The Bhagavad Gita was recited here daily as part of the Ashram schedule.</p>
            

            <p><a href="https://en.wikipedia.org/wiki/Sabarmati_Ashram" target="_blank">Read more</a>to find out more details about sabarmati aashram</p>
        </article>

        <footer>
            &copy;Travel & Tourisam
        </footer>
    </body>
</html>
