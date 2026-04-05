
---
layout: default
title: Ahmed Munawar Portfolio
---

<header>
    <div class="container">
        <div class="row">
            <div class="col-lg-12">
                <img class="img-responsive" src="{{ '/assets/img/profile.png' | relative_url }}" alt="Ahmed Munawar">
                <div class="intro-text">
                    <span class="name">Ahmed Munawar</span>
                    <hr class="star-light">
                    <span class="skills">Computer Engineering Student - Tech Explorer - Programmer</span>
                </div>
            </div>
        </div>
    </div>
</header>

<section id="portfolio">
    <div class="container">
        <div class="row">
            <div class="col-lg-12 text-center">
                <h2>Portfolio</h2>
                <hr class="star-primary">
            </div>
        </div>
        <div class="row">
            {% for project in site.portfolio %}
            <div class="col-sm-4 portfolio-item">
                <a href="#portfolioModal{{ forloop.index }}" class="portfolio-link" data-toggle="modal">
                    <div class="caption">
                        <div class="caption-content">
                            <i class="fa fa-search-plus fa-3x"></i>
                        </div>
                    </div>
                    <img src="{{ project.img | relative_url }}" class="img-responsive" alt="{{ project.title }}">
                </a>
            </div>
            {% endfor %}
        </div>
    </div>
</section>
