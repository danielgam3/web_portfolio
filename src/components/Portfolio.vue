<template>
  <div class="hello">
    <head>
      <title>Graphic Designer Portfolio</title>
    </head>
    <body>
      <header>
        <h1>Portfolio of Daniel Gamez</h1>
      </header>
      <main>
        <section class="projects_section">
          <h2>Some designs I worked on</h2>
          <div class="project-container">
            <div class="project">
              <img src="../assets/project-preview-small.png" class="geometric_design" alt="project 1">
              <h3>Geometric design</h3>
            </div>
            <div class="project">
              <img src="../assets/post-thumbnail.png" alt="Project 2">
              <h3>Rocket logo</h3>
            </div>
            <div class="project">
              <img src="../assets/d80f95fbe24ed0f505630743f287332b.jpg" alt="Project 3">
              <h3>Sun design</h3>
            </div>
            <div class="project">
              <img src="../assets/Astro.jpeg" class="astronaut_design" alt="project 4">
              <h3>Astro design</h3>
            </div>
            <div class="project">
              <img src="../assets/business.jpg" class="business_design" alt="project 5">
              <h3>Business design</h3>
            </div>
          </div>
        </section>
        <section>
          <h2>Business Card</h2>
          <div class="business-card-container">
            <div class="business-card">
              <img src="../assets/business-card-front.png" alt="Business Card Front">
              <img src="../assets/business-card-back.png" alt="Business Card Back">
            </div>
          </div>
        </section>
        <section class="cv_section">
          <h2>CV</h2>
          <p>Click the button below to view my PDF CV:</p>
          <a href="https://drive.google.com/file/d/1c8lASiGGqGgi22snn5PzlIoZ2r5rM4ps/view?usp=sharing">View PDF CV</a>
          <p>Watch my CV video on YouTube:</p>
          <a href="https://youtu.be/79T7AktXlnc" target="_blank" rel="noopener noreferrer">View CV Video</a>
        </section>
        <section class="about_me_section">
          <h2>About Me</h2>
          <p>Hi there! I'm a passionate graphic designer currently studying at EASV Esbjerg in Denmark. My love for design began when I was young, and has only grown stronger over the years. I enjoy experimenting with different styles and techniques, and I'm always looking for new and innovative ways to bring my ideas to life. Whether I'm working on a logo, a website, or a branding project, my goal is always the same: to create designs that not only look great, but also effectively communicate the message and vision of my clients. When I'm not designing, you can usually find me exploring the beautiful Danish countryside or experimenting with new recipes in the kitchen.</p>
        </section>
        <section class="contact_section">
          <h2>Contact</h2>
          <ul>
            <li>Email: danielgamezgonzalez6@gmail.com</li>
            <li><a href="https://www.linkedin.com/in/daniel-g%C3%A1mez-gonz%C3%A1lez-522218269/">LinkedIn</a></li>
          </ul>
        </section>
      </main>
    </body>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
body {
  margin: 0;
  font-family: sans-serif;
  background-image: linear-gradient(to bottom right, #ffffff, #b7acde);
  font-family: 'Open Sans', sans-serif;
  font-weight: 400;
}

header {
  background-color: black;
  color: #fff;
  text-align: center;
  padding: 20px;
  background-color: black;
  color: #fff;
  text-align: center;
  animation: fadeInDown 3s ease;
}

@keyframes fadeInDown {
  0% {
    opacity: 0;
    transform: translateY(-20px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

main {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
}

section {
  width: 100%;
  max-width: 800px;
  margin-bottom: 40px;
}

h2 {
  margin-top: 50px;
  margin-bottom: 50px;
  width: max-content;
  font-weight: 600;
}

.project-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.project {
  width: 300px;
  margin: 20px;
  text-align: center;
}

.project img:hover {
  transform: scale(1.1);
  transition: transform 0.3s ease-in-out;
}

.geometric_design{
  height: 169px;
}

.astronaut_design{
  height: 300px;
}

.project img {
  width: 100%;
}

@media screen and (max-width: 480px) {
  .project {
    width: 100%;
  }
}

.business-card-container {
  display: flex;
  justify-content: center;
}

.business-card {
  width: 600px;
  display: flex;
  justify-content: space-between;
}

.business-card img {
  width: 280px;
  border: 1px solid #333;
}

@media screen and (max-width: 480px) {
  .business-card {
    flex-direction: column;
    align-items: center;
  }

  .business-card img {
    margin-bottom: 20px;
    border: 1px solid #333;
  }
}

.cv_section {
  background-color: black;
  border: 1px solid #ddd;
  border-radius: 20px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  margin-bottom: 20px;
  padding: 20px;
  width: max-content;
}

.cv_section h2 {
  color: white;
  margin-left: 43%;
  font-size: 24px;
  font-weight: 700;
  margin-bottom: 10px;
  text-transform: uppercase;
}

.cv_section p {
  color: white;
  font-size: 16px;
  line-height: 1.5;
  margin-bottom: 20px;
}

.cv_section a {
  background-color: #007bff;
  border: none;
  border-radius: 20px;
  color: #fff;
  display: inline-block;
  font-size: 16px;
  font-weight: 700;
  margin-right: 10px;
  padding: 10px 20px;
  text-decoration: none;
  text-transform: uppercase;
  transition: all 0.3s ease;
}

.cv_section a:hover {
  background-color: #0069d9;
  color: #fff;
}

.cv_section a:active {
  transform: translateY(2px);
}

.about_me_section{
  padding: 50px 20px;
  border: 1px solid #ddd;
  color: #333;
  font-size: 18px;
  border-radius: 20px;
  background-color: black;
}
.about_me_section h2{
  color: white;
  margin-left: 43%;
}
.about_me_section P{
  color: white;
}

.contact_section {
  background-color: black;
  padding: 50px 20px;
  color: #333;
  font-size: 18px;
  border-radius: 20px;
  margin-bottom: 0%;
  border: 1px solid #ddd;
}

.contact_section h2 {
  font-size: 24px;
  margin-bottom: 20px;
  margin-left: 43%;
  color: white;
}

.contact_section ul {
  margin: 0;
  padding: 0;
  list-style: none;
  text-align: center;
}

.contact_section li {
  margin-bottom: 10px;
  color: white;
}

.contact_section a{
  background-color: #007bff;
  border: none;
  border-radius: 20px;
  color: #fff;
  display: inline-block;
  font-size: 16px;
  font-weight: 700;
  margin-right: 10px;
  padding: 10px 20px;
  text-decoration: none;
  text-transform: uppercase;
  transition: all 0.3s ease;
}

.contact_section a:hover {
  background-color: #0069d9;
  color: #fff;
}

.contact_section a:active {
  transform: translateY(2px);
}
</style>
