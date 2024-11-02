---
order: 5
include: section.html
class: portfolio section
sid: portfolio
---

<h2 class="section__title">Portfolio</h2>
<span class="section__subtitle">Recent works</span>

<div class="portfolio__container container swiper-container">

    <div class="swiper-wrapper">

        {% for portfolio in site.data.portfolios %}
        <div class="portfolio__content grid swiper-slide">
            <img src="{{ portfolio.img }}" alt="" class="portfolio__img">

            <div class="portfolio__data">
                <h3 class="portfolio__title">{{ portfolio.title }}</h3>
                <p class="portfolio__description">
                    {{ portfolio.description }}
                </p>
                <a href="{{ portfolio.href }}" class="button button--flex button--small portfolio__button">
                    {{ portfolio.href_text }}
                    <i class="uil uil-{{ portfolio.icon }} button__icon"></i>
                </a>
            </div>
        </div>
        {% endfor %}

    </div>

    <!-- Add Arrows -->
    <div class="swiper-button-next">
        <i class="uil uil-angle-right-b  swiper-portfolio-icon"></i>
    </div>

    <div class="swiper-button-prev">
        <i class="uil uil-angle-left-b  swiper-portfolio-icon"></i>
    </div>

    <!-- Add Pagination -->
    <div class="swiper-pagination"></div>
</div>
