---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---
<section id="wrapper">

  <!-- One -->
  <section id="one" class="wrapper spotlight style1">
    <div class="inner">
      <img class="image" src="{{ "/assets/img/Luis_Estrada.jpg" }}" alt="Me" />
      <div class="content">
        <h2 class="major">About me</h2>
        <p>
        Hi! I'm Luis. I'm a software developer from the Bay Area and I love to code.
        <br>
        I studied at San Francisco State University where I learned many of the fundamentals of Computer Science and gained lots of experience working collaboratively with others.
        <br>
        I started school with very little exposure to coding and ended up finishing my capstone Software Engineering course as lead developer of my team.
        <br>
        After graduating, I joined the Mission Techies training program at MEDA to further sharpen my technical and professional skills.
        <br>
        Lately, I've been teaching myself new technologies and am taking a course on Udacity as part of the Grow with Google scholarship for Front-End Development.
        <br>
        I'm currently looking for new opportunities to reach my goal of being a full-stack developer and to help your teams build great products.
        </p>
        <a href="https://linkedin.com/in/{{ site.linkedin_username }}" class="special">Learn more</a>
      </div>
    </div>
  </section>

  <!-- Two -->
  <section id="two" class="wrapper alt style1">
    <div class="inner">
      <h2 class="major">Projects</h2>
      <p>
        During my time at SFSU, I worked on many projects, four of which were team-oriented.
        I've built an Android app, a static web server, an online card game,
        and for my last project, I worked on an e-commerce website as the lead developer of my team.
      </p>
      <p>
        To see more, check out my <a href="https://github.com/{{ site.github_username }}">GitHub</a>.
      </p>
      <section class="features">
        <article>
          <a href="{{ site.url }}{% link projects/shopu.md %}" class="image">
            <img src="{{ "/assets/img/shopu-mod.jpg" | relative_url }}" alt="ShopU logo" />
          </a>
          <h3 class="major">ShopU</h3>
          <p>E-commerce website that provides consumer-to-consumer sales services to SFSU students.<br>Jun 2016 - Aug 2016</p>
          <a href="{{ site.url }}{% link projects/shopu.md %}" class="special">Learn more</a>
        </article>
        <article>
          <a href="{{ site.url }}{% link projects/exploding-kittens.md %}" class="image">
            <img src="{{ "/assets/img/exploding-kittens.jpg" | relative_url }}" alt="Exploding Kittens screenshot" />
          </a>
          <h3 class="major">Exploding Kittens card game</h3>
          <p>Online turn-based card game based on the game of the same name.<br>Apr 2016 - Jun 2016</p>
          <a href="{{ site.url }}{% link projects/exploding-kittens.md %}" class="special">Learn more</a>
        </article>
        <article>
          <a href="{{ site.url }}{% link projects/web-server.md %}" class="image">
            <img src="{{ "/assets/img/server-workflow.png" | relative_url }}" alt="Server workflow diagram" />
          </a>
          <h3 class="major">Static web server</h3>
          <p>Multithreaded static web server written in Ruby to learn about the HTTP protocol.<br>Feb 2016 - Apr 2016</p>
          <a href="{{ site.url }}{% link projects/web-server.md %}" class="special">Learn more</a>
        </article>
        <article>
          <a href="{{ site.url }}{% link projects/parksf.md %}" class="image">
            <img src="{{ "/assets/img/parksf.jpg" | relative_url }}" alt="ParkSF splash screen" />
          </a>
          <h3 class="major">ParkSF Android app</h3>
          <p>Android mobile app that allows users to find and interact with data on parking locations around downtown SF.<br>Feb 2015 - May 2015</p>
          <a href="{{ site.url }}{% link projects/parksf.md %}" class="special">Learn more</a>
        </article>
      </section>
      <ul class="actions">
        <li><a href="{{ site.url }}{% link navigation/projects.md %}" class="button">Browse All</a></li>
      </ul>
    </div>
  </section>

</section>
