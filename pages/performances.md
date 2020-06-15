---
layout: default
title: "Performances"
permalink: "/performances/"
performances:
  - performance_date: 24 JUL 2020
    performance_title: The Book of Etiquette
    venue: N.E.O. Voice Festival
    performers: Tiffany-Alaine Solinap Militante, soprano; Abraham Ross, piano
    url: http://www.neovoicefestival.com/
  - performance_date: 5 MAR 2020
    performance_title: Marvels of Creatures and Strange Things Existing (excerpts) - Reading
    venue: UCLA
    city_state: Los Angeles, CA
    performers: Jihye Chang, piano
  - performance_date: 25 FEB 2020
    performance_title: Migration Variations - Premiere
    venue: UCLA
    city_state: Los Angeles, CA
    performers: Veola Sun, piano 1; Brandon Zhou, piano 2; Robby Good, perc. 1; Cash Langi, perc. 2
  - performance_date: 23 NOV 2019
    performance_title: Migration Variations - Reading
    venue: UCLA
    city_state: Los Angeles, CA
    performers: Yarn/Wire
  - performance_date: 5 NOV 2019
    performance_title: Variations on &quot;This Land is Your Land&quot;
    venue: UCLA
    city_state: Los Angeles, CA
    performers: Christian Gonzales, violin; Austin Ho, piano
  - performance_date: 1 AUG 2019
    performance_title: Variations on &quot;This Land is Your Land&quot; - Premiere
    venue: Montecito Music Festival
    city_state: Los Angeles, CA
    performers: Luiz Paulo Friere, violin; Ji Hyun Ryu, piano
header:
    image_fullwidth_staff: gif-test.gif
---
<div class="row">
	<div class="large-5 columns">
			<header>
				<div class="text-center">
					<h2>Upcoming Performances</h2>
				</div>
			</header>
            <div>
                {% capture now %}{{'now' | date: '%s' | plus: 0 }}{% endcapture %}
                {% for item in page.performances %}
                {% capture date %}{{item.performance_date | date: '%s' | plus: 0 }}{% endcapture %}
                {% if date > now %}
                <hr>
                <ul class="no-bullet">
                    <li><strong>{{ item.performance_date }}</strong></li>
                    {% for work in site.works %}
                    {% if item.performance_title contains work.title %}
                    {% capture not-title %}
                    {{ item.performance_title | remove: work.title }}
                    {% endcapture %}
                    <li><a href="{{ site.url }}{{ site.baseurl }}{{ work.url }}">{{ work.title }}</a>{{not-title}}</li>
                    {% endif %}
                    {% endfor %}
                    {% if not-title == NULL %}
                    <li>{{ item.performance_title }}</li>
                    {% endif %}
                    {% if item.venue %}
                    <li>{{ item.venue }}</li>
                    {% endif %}
                    {% if item.city_state %}
                    <li>{{ item.city_state }}</li>
                    {% endif %}
                    {% if item.performers %}
                    <li>{{ item.performers }}</li>
                    {% endif %}
                    {% if item.url %}
                    <li><a href="{{ item.url }}" target="_blank">More information ›</a></li>
                    {% endif %}
                </ul>
                {% endif %}
                {% endfor %}
            </div>
	</div><!-- /.medium-6.columns -->
    <div class="large-5 columns">
            <header>
				<div itemprop="name" class="text-center">
					<h2>Recent Performances</h2>
				</div>
			</header>
            <div>
                {% capture now %}{{'now' | date: '%s' | plus: 0 }}{% endcapture %}
                {% for item in page.performances %}
                {% capture date %}{{item.performance_date | date: '%s' | plus: 0 }}{% endcapture %}
                {% if date < now %}
                <hr>
                <ul class="no-bullet">
                    <li><strong>{{ item.performance_date }}</strong></li>
                    {% for work in site.works %}
                    {% if item.performance_title contains work.title %}
                    {% capture not-title %}
                    {{ item.performance_title | remove: work.title }}
                    {% endcapture %}
                    <li><a href="{{ site.url }}{{ site.baseurl }}{{ work.url }}">{{ work.title }}</a>{{not-title}}</li>
                    {% endif %}
                    {% endfor %}
                    {% if not-title == NULL %}
                    <li>{{ item.performance_title }}</li>
                    {% endif %}
                    {% if item.venue %}
                    <li>{{ item.venue }}</li>
                    {% endif %}
                    {% if item.city_state %}
                    <li>{{ item.city_state }}</li>
                    {% endif %}
                    {% if item.performers %}
                    <li>{{ item.performers }}</li>
                    {% endif %}
                    {% if item.url %}
                    <li><a href="{{ item.url }}" target="_blank">More information ›</a></li>
                    {% endif %}
                </ul>
                {% endif %}
                {% endfor %}
            </div>
    </div><!-- /.medium-6.columns -->
</div><!-- /.row -->
