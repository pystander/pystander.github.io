---
order: 5
include: sections.html
class: portfolio section
sid: portfolio
---

<h2 class="section__title">Portfolio</h2>
<span class="section__subtitle">Recent works</span>

<div class="portfolio__container container swiper-container">

    <div class="swiper-wrapper">
        <!--==================== PORTFOLIO 1 ====================-->
        <div class="portfolio__content grid swiper-slide">
            <img src="assets/img/word_sea.png" alt="" class="portfolio__img">

            <div class="portfolio__data">
                <h3 class="portfolio__title">Word Sea</h3>
                <p class="portfolio__description">
                    A simple Python app for self-learning English vocabularies.
                </p>
                <a href="https://github.com/pystander/Word-Sea" class="button button--flex button--small portfolio__button">
                    GitHub
                    <i class="uil uil-github button__icon"></i>
                </a>
            </div>
        </div>

        <!--==================== PORTFOLIO 2 ====================-->
        <div class="portfolio__content grid swiper-slide">
            <img src="assets/img/road_to_castle_3d.png" alt="" class="portfolio__img">

            <div class="portfolio__data">
                <h3 class="portfolio__title">The Road to Castle 3D</h3>
                <p class="portfolio__description">
                    A 3D rework of The Road to Castle, originally a text-based RPG on Linux.
                </p>
                <a href="https://wp2023.cs.hku.hk/fyp23002/" class="button button--flex button--small portfolio__button">
                    Website
                    <i class="uil uil-external-link-alt button__icon"></i>
                </a>
            </div>
        </div>

        <!--==================== PORTFOLIO 3 ====================-->
        <div class="portfolio__content grid swiper-slide">
            <img src="assets/img/pacman_game.gif" alt="" class="portfolio__img">

            <div class="portfolio__data">
                <h3 class="portfolio__title">Berkeley-AI-Pacman</h3>
                <p class="portfolio__description">
                    The Pac-Man AI Projects from UC Berkeley CS188 materials.
                </p>
                <a href="https://github.com/pystander/Berkeley-AI-Pacman" target="_blank" class="button button--flex button--small portfolio__button">
                    GitHub
                    <i class="uil uil-github button__icon"></i>
                </a>
            </div>
        </div>
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
