---
order: 4
include: section.html
class: qualification section
sid: qualification
---

<h2 class="section__title">Qualification</h2>
<span class="section__subtitle">My personal journey</span>

<!-- <div class="qualification__description">
    My life has never been smooth sailing.

    <br><br>

    There were times when I was lost and confused,

    <br><br>

    but these setbacks and scars had taught me resilience.
</div> -->

<div class="qualification__container container">

    <div class="qualification__tabs">
        <div class="qualification__button button--flex qualification__active" data-target="#education">
            <i class="uil uil-graduation-cap qualification__icon"></i>
            Education
        </div>

        <div class="qualification__button button--flex" data-target="#work">
            <i class="uil uil-briefcase-alt qualification__icon"></i>
            Work
        </div>
    </div>

    <div class="qualification__sections">

    {% for content in site.data.qualifications %}

        {% if forloop.first == true %}
            <div class="qualification__content qualification__active" data-content id="{{ content.id }}">
        {% else %}
            <div class="qualification__content" data-content id="{{ content.id }}">
        {% endif %}

        {% for qualification in content.details %}
            {% assign remainder = forloop.index | modulo: 2 %}

            <div class="qualification__data">

                {% if remainder == 1 %}
                    <div></div>

                    <div>
                        <span class="qualification__rounter"></span>
                        <span class="qualification__line"></span>
                    </div>
                {% endif %}

                <div>
                    <h3 class="qualification__title">{{ qualification.title }}</h3>
                    <span class="qualification__subtitle">{{ qualification.subtitle }}</span>
                    <div class="qualification__calendar">
                        <i class="uil uil-calendar-alt"></i>
                        {{ qualification.date }}
                    </div>
                </div>

                {% if remainder == 0 %}
                    <div>
                        <span class="qualification__rounter"></span>
                        <span class="qualification__line"></span>
                    </div>
                {% endif %}

            </div>
        {% endfor %}

        </div>
    {% endfor %}

    </div>
</div>
