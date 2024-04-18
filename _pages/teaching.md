---
layout: page
permalink: /teaching/
title: teaching
nav: true
nav_order: 5
years: [2024, 2023, 2022, 2021, 2020, 2019, 2018]
---
<div class="projects">
    {%- for year in page.years %}
        {%- assign courses = site.data.teaching | where: "year", year -%}
        <h2 class="category"> {{ year }} </h2>
            <div class="grid">
                {%- for course in courses %}
                    {%- include course.html %}
                {%- endfor %}
            </div>
    {%- endfor %}
</div>

