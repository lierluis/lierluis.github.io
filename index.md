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
      <a href="#" class="image"><img src="images/pic01.jpg" alt="" /></a>
      <div class="content">
        <h2 class="major">About me</h2>
        <p>
        I'm a software engineer with a passion for technology and programming.
        I recently graduated from San Francisco State University with a B.S. in
        Computer Science, and have over 3 years of programming experience.
        I also recently graduated from the Mission Techies program at MEDA
        where I prepared for a professional career in the tech industry.
        I'm currently looking for new opportunities to continue my career
        in software development.
        If you'd like to see some of my work, check out my <a href="{{ site.url }}{% link navigation/projects.md %}">projects</a>.
        </p>
        <a href="#" class="special">Learn more</a>
      </div>
    </div>
  </section>

  <!-- Two -->
  <section id="two" class="wrapper alt style1">
    <div class="inner">
      <h2 class="major">Projects</h2>
      <p>Cras mattis ante fermentum, malesuada neque vitae, eleifend erat. Phasellus non pulvinar erat. Fusce tincidunt, nisl eget mattis egestas, purus ipsum consequat orci, sit amet lobortis lorem lacus in tellus. Sed ac elementum arcu. Quisque placerat auctor laoreet.</p>
      <section class="features">
        <article>
          <a href="{{ site.url }}{% link projects/shopu.md %}" class="image">
            <img src="{{ "/assets/img/shopu-mod.jpg" | relative_url }}" alt="ShopU logo" />
          </a>
          <h3 class="major">ShopU</h3>
          <p>Mock e-commerce website that provides consumer-to-consumer sales services to SFSU students.<br>Jun 2016 - Aug 2016</p>
          <a href="#" class="special">Learn more</a>
        </article>
        <article>
          <a href="{{ site.url }}{% link projects/exploding-kittens.md %}" class="image">
            <img src="{{ "/assets/img/exploding-kittens.jpg" | relative_url }}" alt="Exploding Kittens screenshot" />
          </a>
          <h3 class="major">Exploding Kittens card game</h3>
          <p>Online turn-based card game based on the game of the same name.<br>Apr 2016 - Jun 2016</p>
          <a href="#" class="special">Learn more</a>
        </article>
        <article>
          <a href="{{ site.url }}{% link projects/web-server.md %}" class="image">
            <img src="{{ "/assets/img/server-workflow.png" | relative_url }}" alt="Server workflow diagram" />
          </a>
          <h3 class="major">Static web server</h3>
          <p>Multithreaded static web server written in Ruby to learn about the HTTP protocol.<br>Feb 2016 - Apr 2016</p>
          <a href="#" class="special">Learn more</a>
        </article>
        <article>
          <a href="{{ site.url }}{% link projects/parksf.md %}" class="image">
            <img src="{{ "/assets/img/parksf.jpg" | relative_url }}" alt="ParkSF splash screen" />
          </a>
          <h3 class="major">ParkSF Android app</h3>
          <p>Android mobile app that allows users to find and interact with data on parking locations around downtown SF.<br>Feb 2015 - May 2015</p>
          <a href="#" class="special">Learn more</a>
        </article>
      </section>
      <ul class="actions">
        <li><a href="{{ site.url }}{% link navigation/projects.md %}" class="button">Browse All</a></li>
      </ul>
    </div>
  </section>

</section>
