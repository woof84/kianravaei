---
layout: default
title: "Performances"
permalink: "/performances/"
performances:
  - performance_date: 22 Jun 2021
    performance_title: Family Photos
    venue: Salastina Happy Hour No. 62, Sounds Promising World Premieres (Livestream)
    performers: Salastina
    url: https://www.salastina.org/concerts/2021/6/22/happy-hour-no-62-sounds-promising-world-premieres-part-1
  - performance_date: 15 Jun 2021
    performance_title: Lotf Nemīkhâm
    venue: Suoni Per Il Popolo
    city_state: Deterritorializing the Realm of New Music (Livestream)
    performers: Anoush Moazenni, speaking pianist
    url: https://suoniperilpopolo.org/en/program/anoush-moazzeni
  - performance_date: 10 Jun 2021
    performance_title: Family Photos - Premiere
    venue: EMERGE Virtual Concert (Livestream)
    performers: The Julius Quartet
  - performance_date: 7 Jun 2021
    performance_title: Written by Children - Premiere
    venue: UCLA (Livestream)
    city_state: Los Angeles, California
    performers: Rachel Boehl, horn
  - performance_date: 26 May 2021
    performance_title: Marvels of Creatures and Strange Things Existing (excerpt)
    venue: UCLA (Livestream)
    city_state: Los Angeles, California
    performers: Kennethe Glendon Brown, piano
    url: https://schoolofmusic.ucla.edu/event/the-inaugural-selma-moidel-smith-recital/?mc_cid=c4f757510c&mc_eid=5fdf70357e
  - performance_date: 27 APR 2021
    performance_title: Ideal Conversation
    venue: UCLA (Livestream)
    city_state: Los Angeles, California
    performers: Julia Johnson, voice; Valerie Stern, piano
    url:
  - performance_date: 27 APR 2021
    performance_title: Advertisements (excerpts)
    venue: UCLA (Livestream)
    city_state: Los Angeles, California
    performers: Kian Ravaei, voice and guitar; Justin Birchell, baritone; Joseph Seyedan, guitar
    url:
  - performance_date: 19 MAR 2021
    performance_title: Prisoners of Hope
    venue: UCLA (Livestream)
    city_state: Los Angeles, California
    performers: Jocelyn Yeh, cello
    url:
  - performance_date: 6 MAR 2021
    performance_title: Prelude and Fugue in C-Sharp - Premiere
    venue: UCLA (Livestream)
    city_state: Los Angeles, California
    performers: Stefano Greco, piano
    url:
  - performance_date: 16 FEB 2021
    performance_title: Prisoners of Hope - Premiere
    venue: UCLA (Livestream)
    city_state: Los Angeles, California
    performers: Jocelyn Yeh, cello
    url:
  - performance_date: 31 JAN 2021
    performance_title: Advertisements - Premiere
    venue: KC VITAs VOICES OF VITAs (Livestream)
    city_state: Kansas City, Kansas
    performers: Patrick Graham, baritone; Aleia Gonzales Gulino, guitar
    url: https://www.kcvitas.org/
  - performance_date: 18 DEC 2020
    performance_title: A Little Consort Music
    venue: UCLA (Livestream)
    city_state: Los Angeles, California
    performers: Calvin Kung, Jocelyn Yeh, Peter Walsh; cello
    url: https://www.youtube.com/watch?v=Dz69toVdBuU
  - performance_date: 12 DEC 2020
    performance_title: Caprice
    venue: UCLA (Livestream)
    city_state: Los Angeles, California
    performers: Lavinia Chen, violin; Christopher Ye, cello
    url:
  - performance_date: 27 NOV 2020
    performance_title: A Little Consort Music - European Premiere
    venue: Festival Osmose
    city_state: Espace Toots, Belgium
    performers: Alexandre Debrus, Bruno Ispiola, Johannes Burghoff; cello
    url:
  - performance_date: 10 NOV 2020
    performance_title: A Little Consort Music - Premiere
    venue: UCLA (Livestream)
    city_state: Los Angeles, California
    performers: Calvin Kung, Jocelyn Yeh, Peter Walsh; cello
    url: 
  - performance_date: 10 NOV 2020
    performance_title: Caprice - Premiere
    venue: UCLA (Livestream)
    city_state: Los Angeles, California
    performers: Lavinia Chen, violin; Christopher Ye, cello
    url: 
  - performance_date: 29 AUG 2020
    performance_title: Sestina - Premiere
    venue: Curtis Institute of Music Young Artist Summer Program Young Composers Marathon
    performers: Paul Demers, bass clarinet
    url:
  - performance_date: 25 JUL 2020
    performance_title: Ideal Conversation - Premiere
    venue: N.E.O. Voice Festival (Livestream)
    city_state: Los Angeles, California
    performers: Tiffany-Alaine Solinap Militante, voice; Abraham Ross, piano
    url: https://voicescienceworks.ticketspice.com/neo-voice-festival-weekend-2020
  - performance_date: 6 MAR 2020
    performance_title: Duo for Trombone and Piano - Premiere
    venue: UCLA
    city_state: Los Angeles, CA
    performers: Gwang Hyun Kim, trombone; Hana Kim, piano
    url:
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
    image_fullwidth_staff: Kian_Header_idea_9.png
---


<!--Same margins as page-->

<div class="row t30">
	<div class="medium-8 columns medium-offset-2 end">

<!--Upcoming performances-->

<div class="text-center">
					<h1 class="h">Upcoming Performances</h1>
				</div>
                {% capture now %}{{'now' | date: '%s' | plus: 0 }}{% endcapture %}
                {% assign i = 0 %}
                {% for item in page.performances %}
                {% capture date %}{{item.performance_date | date: '%s' | plus: 0 }}{% endcapture %}
                {% if date > now %}
                {% assign i = i | plus:1 %}
                <hr>
<div class="row">
                    
  <div class="small-5 columns">
    <p class="performance-date text-right">{{ item.performance_date }}</p>
    </div>
    <div class="small-7 columns">
    <ul class="no-bullet">
        {% for work in site.works %}
                    {% if item.performance_title contains work.title %}
                    {% capture not-title %}
                    {{ item.performance_title | remove: work.title }}
                    {% endcapture %}
                    <li style="font-size:20px;"><b><a href="{{ site.url }}{{ site.baseurl }}{{ work.url }}">{{ work.title }}</a>{{not-title}}</b></li>
                    {% endif %}
                    {% endfor %}
                    {% if not-title == NULL %}
                    <li style="font-size:20px;"><b>{{ item.performance_title }}</b></li>
                    {% endif %}
                    {% if item.venue %}
                    <li style="color:dimgray;">{{ item.venue }}</li>
                    {% endif %}
                    {% if item.city_state %}
                    <li style="color:dimgray;">{{ item.city_state }}</li>
                    {% endif %}
                    {% if item.performers %}
                    <li style="color:dimgray;">{{ item.performers }}</li>
                    {% endif %}
                    {% if item.url %}
                    <li style="margin-top:10px;"><a class="button tiny round" href="{{ item.url }}" target="_blank">More Information ›</a></li>
                    {% endif %}
      </ul>
      </div>
    </div>
      {% endif %}
                {% endfor %}
    {% if i == 0 %}
    <p class="text-center teaser" style="color:dimgray;">No upcoming performances.</p>
    {% endif %}


<!--Recent performances-->


<div class="text-center t30">
					<h1 class="h1">Recent Performances</h1>
				</div>
    {% capture now %}{{'now' | date: '%s' | plus: 0 }}{% endcapture %}
                {% for item in page.performances %}
                {% capture date %}{{item.performance_date | date: '%s' | plus: 0 }}{% endcapture %}
                {% if date < now %}
<div class="row">
                    <hr>
  <div class="small-5 columns">
    <p class="performance-date text-right">{{ item.performance_date }}</p>
    </div>
  <div class="small-7 columns">
    <ul class="no-bullet">
        {% for work in site.works %}
                    {% if item.performance_title contains work.title %}
                    {% capture not-title %}
                    {{ item.performance_title | remove: work.title }}
                    {% endcapture %}
                    <li style="font-size:20px;"><b><a href="{{ site.url }}{{ site.baseurl }}{{ work.url }}">{{ work.title }}</a>{{not-title}}</b></li>
                    {% endif %}
                    {% endfor %}
                    {% if not-title == NULL %}
                    <li style="font-size:20px;"><b>{{ item.performance_title }}</b></li>
                    {% endif %}
                    {% if item.venue %}
                    <li style="color:dimgray;">{{ item.venue }}</li>
                    {% endif %}
                    {% if item.city_state %}
                    <li style="color:dimgray;">{{ item.city_state }}</li>
                    {% endif %}
                    {% if item.performers %}
                    <li style="color:dimgray;">{{ item.performers }}</li>
                    {% endif %}
      </ul>
      </div>
    </div>
      {% endif %}
                {% endfor %}


</div>
</div>
