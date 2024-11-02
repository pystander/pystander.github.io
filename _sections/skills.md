---
order: 3
include: section.html
class: skills section
sid: skills
---

<h2 class="section__title">Skills</h2>
<span class="section__subtitle">My technical levels</span>

<div class="skills__container container grid">

    {% for skill in site.data.skills %}
    <!--==================== SKILL ====================-->
    <div class="skills__content skills__close">
        <div class="skills__header">
            <i class="uil uil-{{ skill.icon }} skills__icon"></i>

            <div>
                <h1 class="skills__title">{{ skill.title }}</h1>
                <span class="skills__subtitle">{{ skill.subtitle }}</span>
            </div>

            <i class="uil uil-angle-down skills__arrow"></i>
        </div>

        <div class="skills__list grid">

            {% for detail in skill.details %}
            <div class="skills__data">
                <div class="skills__titles">
                    <h3 class="skills__name">{{ detail.name }}</h3>
                    <span class="skills__number">{{ detail.percentage }}</span>
                </div>

                <div class="skills__bar">
                    <span class="skills__percentage" style="width: {{ detail.percentage }}"></span>
                </div>
            </div>
            {% endfor %}

        </div>
    </div>
    {% endfor %}

</div>
