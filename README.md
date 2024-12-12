<!DOCTYPE html>
<html>
    <head>
        <style>
            *{
                text-align:center;
            }
            .heading{
                background-color:orange;
                color:white;
                padding:10px;
            }
            footer{
                background-color:black;
                color:white;
            }
            body {
                font-family: Arial, sans-serif;
                margin: 0;
                background-color: #f4f4f4;
              }

            .slideshow-container {
              position: relative;
              max-width: 800px;
              margin: 50px auto;
              overflow: hidden;
              border-radius: 10px;
            }

            .slide {
              display: none;
              position: relative;
            }

            .slide img {
              width: 100%;
              display: block;
            }

            .caption {
              position: absolute;
              bottom: 10px;
              left: 10px;
              color: #fff;
              background-color: rgba(0, 0, 0, 0.6);
              padding: 5px 10px;
              border-radius: 5px;
            }

            .prev, .next {
              cursor: pointer;
              position: absolute;
              top: 50%;
              width: auto;
              margin-top: -22px;
              padding: 16px;
              color: white;
              font-weight: bold;
              font-size: 18px;
              user-select: none;
              background-color: rgba(0, 0, 0, 0.5);
              border: none;
              border-radius: 50%;
            }

            .prev:hover, .next:hover {
              background-color: #555;
            }

            .prev {
              left: 10px;
            }

            .next {
              right: 10px;
            }

            .fade {
              animation-name: fade;
              animation-duration: 1.5s;
            }

            @keyframes fade {
              from {opacity: 0.4;}
              to {opacity: 1;}
            }
        </style>
    </head>
    <body>
        <div class="heading">
            <h1>
                2024 Dev Tours & Travels
            </h1>
            <p>
                Your ultimate travel partner to explore Uttarakhand.
            </p>
        </div>
        <div class="slideshow-container">
    <!-- Slides -->
    <div class="slide fade">
      <img src="https://lp-cms-production.imgix.net/2022-03/GettyRF_956963154.jpg?w=600&h=400" alt="Image 1">
      <div class="caption">The Green Valleys</div>
    </div>
    <div class="slide fade">
      <img src="https://static.toiimg.com/photo/msid-89326554,width-96,height-65.cms" alt="Image 2">
      <div class="caption">An Awesome Mountain View</div>
    </div>
    <div class="slide fade">
      <img src="https://deih43ym53wif.cloudfront.net/Uttarakhand-kedarnath-temple-before-sunrise-hindu-shutterstock_375337813.jpg_d5aae7fdd5.jpg" alt="Image 3">
      <div class="caption">Beautiful Temples On The Mountains</div>
    </div>

    <!-- Navigation buttons -->
    <a class="prev" onclick="changeSlide(-1)">&#10094;</a>
    <a class="next" onclick="changeSlide(1)">&#10095;</a>
  </div>
  <script>
    let slideIndex = 0;
showSlides();

function showSlides() {
  let slides = document.querySelectorAll(".slide");
  slides.forEach(slide => slide.style.display = "none");

  slideIndex++;
  if (slideIndex > slides.length) { slideIndex = 1; }
  slides[slideIndex - 1].style.display = "block";

  setTimeout(showSlides, 3000); // Change image every 3 seconds
}

function changeSlide(n) {
  let slides = document.querySelectorAll(".slide");
  slides[slideIndex - 1].style.display = "none";

  slideIndex += n;
  if (slideIndex > slides.length) { slideIndex = 1; }
  if (slideIndex < 1) { slideIndex = slides.length; }

  slides[slideIndex - 1].style.display = "block";
}
  </script>
        <h2>
            Why Choose us?
        </h2>
        <p>
            At Dev Tours and Travels we serve more. From free trials, to more exciting experiences, we can serve anything.
        </p>
        <footer>
            <p>
                Dev Tour and Travels. | All rights Reserved
            </p>
        </footer>
    </body>
</html>
