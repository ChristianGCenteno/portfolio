---
layout: default
---
<link rel="stylesheet" href="/assets/css/style.css">

<div class="profile-card">
  <h2 class="about-me">ABOUT</h2>
  <img src="{{ site.baseurl }}/assets/img/Main/profile_img.png" alt="Profile photo" class="profile-pic">
  <div class="profile-info">
    <h3>EDUCATION</h3>
    <p><img src="{{ site.baseurl }}/assets/img/Main/uned-ico.png" alt="UNED logo" class="logo-text"> UNED | COMPUTER ENGINEERING DEGREE</p> 

    <h3>PRINCIPAL SKILLS</h3>
    <ul class="ul-to-tag">
      <li class="li-to-tag">Data Engineer</li>
      <li class="li-to-tag">Data Analyst</li>
      <li class="li-to-tag">SQL</li>
      <li class="li-to-tag">Python</li>
      <li class="li-to-tag">PowerBI</li>
    </ul>

    <h3>SUMMARY</h3>
    <p>Former OS Systems and Networking Administrator, currently holding a Computer Engineering degree from the National University of Distance Education (UNED).</p>
    <p>Experience in the insurance sector as a SQL-based backend developer, later transitioning into healthcare as a support technician and data analyst.</p>
    <p>Passionate about innovation, data processing, and emerging technologies. I am proactive, organized, and enjoy collaborating in team environments.</p>

  </div>
</div>

<br>
* * *

<section class="projects">

  <div class="project">
    <div class="project-info">
      <h3>Exploring Cardmarket with Web Scraping</h3> <!-- Project Title -->
      <p>A project that uses web scraping in an e-commerce to create an analytical report using PowerBI.</p>
      <ul class="ul-to-tag">
        <li class="li-to-tag">Python</li>
        <li class="li-to-tag">PowerBI</li>
      </ul>
      <a href="{{ site.baseurl }}/pages/WebScrapCM-pages.html" class="take-look">Take a Look</a>  <!-- <= Where I put the project page -->
    </div>
    <div class="project-img">
      <img src="{{ site.baseurl }}/assets/img/WS-CM/WsMain.png" alt="Ws Picture"> <!-- <= Where I put the project img -->
    </div>
  </div>
 
    <!-- For futures projects, just replicate the structure -->
	
</section>

<!-- END -->
    
<!-- Custom footer -->
<div class="custom-footer" style="text-align: center; padding: 1rem; font-size: 0.8rem; color: gray;">
  We can connect in | 
  <a href="https://www.linkedin.com/in/christian-gabriel-centeno-0b19aa2a1" target="_blank">
    <img src="{{ site.baseurl }}/assets/img/Main/linkedin-ico.png" alt="Linkedin logo" class="logo-text"> Profile
  </a>
</div>

<!-- ANIMATION PROJECT STYLE -->
<script>
  document.addEventListener('DOMContentLoaded', () => {
    const projects = document.querySelectorAll('.project');

    let lastScrollY = window.scrollY;

    const observer = new IntersectionObserver((entries) => {
      const currentScrollY = window.scrollY;
      const scrollingUp = currentScrollY < lastScrollY;
      lastScrollY = currentScrollY;

      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
        } else if (scrollingUp) {
          entry.target.classList.remove('visible');
        }
      });
    }, {
      threshold: 0.2
    });

    projects.forEach(project => {
      observer.observe(project);
    });
  });
</script>