---
layout: default
---
<link rel="stylesheet" href="/assets/css/style.css">

<div class="profile-card">
  <h2 class="about-me">ABOUT ME</h2>
  <img src="{{ site.baseurl }}/assets/img/Main/profile_img.png" alt="Profile photo" class="profile-pic">
  <div class="profile-info">
    <h3>EDUCATION</h3>
    <p><img src="{{ site.baseurl }}/assets/img/Main/uned-ico.png" alt="UNED logo" class="logo-text"> UNED | COMPUTER ENGINEERING</p> 

    <h3>KEY SKILLS</h3>
    <ul class="ul-to-tag">
	  <li class="li-to-tag">Data Analyst</li>
      <li class="li-to-tag">Data Engineer</li>
      <li class="li-to-tag">SQL</li>
      <li class="li-to-tag">Python</li>
      <li class="li-to-tag">PowerBI</li>
    </ul>

    <h3>SUMMARY</h3>
    <p>I'm a freelance Data Specialist based in the Netherlands with a Computer Engineering degree from the National University of Distance Education (UNED).</p>
    <p>I have 4 years of experience across SQL development, BI, data analysis and engineering. My background ranges from building SQL procedures and automating workflows, to creating dashboards in Power BI and supporting data-driven decision making.</p>
    <p>I enjoy adapting quickly to new environments, learning continuously and helping teams turn complex data into actionable insights.</p>

  </div>
</div>

<br>
* * *

<section class="projects">

  <div class="project">
    <div class="project-info">
      <h3>Weather and Pollution Data Visualizer for Dutch Cities</h3> <!-- Project Title -->
      <p>A project that uses API Integration, SQL Translation and GUI Implementation to Visualizer any weather location.</p>
      <ul class="ul-to-tag">
        <li class="li-to-tag">Python</li>
        <li class="li-to-tag">API pipelines</li>
		<li class="li-to-tag">SQLite</li>
		<li class="li-to-tag">PyQt5</li>
      </ul>
      <a href="{{ site.baseurl }}/pages/WeatherAPI-pages.html" class="take-look">Take a Look</a>  <!-- <= Where I put the project page -->
    </div>
    <div class="project-img">
      <img src="{{ site.baseurl }}/assets/img/Weather-API/WAPIMain.png" alt="WAPI Picture"> <!-- <= Where I put the project img -->
    </div>
  </div>

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
