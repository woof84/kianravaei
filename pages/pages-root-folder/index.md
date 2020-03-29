---
layout: default
header: no
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---


<div id="masthead-with-text" style="background: rgba(17,38,91,0.5);">
	<div class="row">
		<div class="large-12 columns">
            <header>
            <div itemprop="name" class="text-center t1" style="background: rgba(214,221,232); border-radius: 20px;">
					<h1 class="custom-site-title">KIAN RAVAEI</h1>
                    <p style="letter-spacing: 2px; font-weight: bold; font-family: 'Ariel', sans-serif; text-shadow: 0 1px 2px rgba(0,0,0,.4); color: black">[<a href="https://en.wikipedia.org/wiki/Voiceless_velar_stop" target="_blank">k</a><a href="https://en.wikipedia.org/wiki/Close_front_unrounded_vowel" target="_blank">i</a><a href="https://en.wikipedia.org/wiki/Voiced_palatal_approximant" target="_blank">j</a><a href="https://en.wikipedia.org/wiki/Open_back_rounded_vowel" target="_blank">&#594;</a><a href="https://en.wikipedia.org/wiki/Voiced_dental,_alveolar_and_postalveolar_nasals" target="_blank">n</a> <a href="https://en.wikipedia.org/wiki/Voiced_dental_and_alveolar_taps_and_flaps" target="_blank">&#638;</a><a href="https://en.wikipedia.org/wiki/Near-open_front_unrounded_vowel" target="_blank">&#230;</a><a href="https://en.wikipedia.org/wiki/Voiced_labiodental_fricative" target="_blank">v</a><a href="https://en.wikipedia.org/wiki/Open_back_rounded_vowel" target="_blank">&#594;</a><a href="https://en.wikipedia.org/wiki/Vowel_length" target="_blank">&#720;</a><a href="https://en.wikipedia.org/wiki/Close_front_unrounded_vowel" target="_blank">i</a><a href="https://en.wikipedia.org/wiki/Vowel_length" target="_blank">&#720;</a>]<br>&nbsp;</p>
            </div>
        </header>
		</div><!-- /.small-12.columns -->
	</div><!-- /.row -->
</div><!-- /#masthead -->

<div class="row t60">
    <div class="large-12 columns">
        <p style="font-size: 20px;">Born (1999) and raised in Los Angeles, <strong>Kian Ravaei</strong> has written for a variety of ensembles ranging from chamber to choral to orchestral. His recent work aims to shed light upon political events past and present, addressing topics such as national identity, migration, and commercialism. <a href="{{ site.url }}{{ site.baseurl }}/works/">Full Bio ></a></p>
	</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
<div class="row">
    <div class="medium-6 columns medium-push-6">
                <h2 style="text-align: center">Upcoming Performances</h2>
                {% for page in site.pages %}
                    {% if page.title == "Performances" %}
                        {% for item in page.performances %}
                {% capture now %}{{'now' | date: '%s' | plus: 0 }}{% endcapture %}
                {% capture date %}{{item.performance_date | date: '%s' | plus: 0 }}{% endcapture %}
                {% if date > now %}
                <ul class="no-bullet">
                    <li>&nbsp;</li>
                    <li><strong>{{ item.performance_date }}</strong></li>
                    {% if item.performance_title %}
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
                </ul>
                <ul class="side-nav"><li class="divider"></li></ul>
                {% endif %}
                {% endfor %}
                    {% endif %}
                {% endfor %}
        <p style="text-align: right">&nbsp;<br><a href="{{ site.url }}{{ site.baseurl }}/performances/">All Performances ></a></p>
    </div>
    <div class="medium-6 columns medium-pull-6">
        <h2 style="text-align: center">Recent Works</h2>
        <ul class="side-nav">
        {% for post in site.categories.works limit: 3 %}
        <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{% if post.subheadline %}{{ post.subheadline }} &middot; {% endif %}<strong>{{ post.title }}</strong><br><span style="color: #000000;">{{ post.year_composed }}/For {{ post.instrumentation }}</span></a></li>
        {% endfor %}
        </ul>
        <p style="text-align: right"><a href="{{ site.url }}{{ site.baseurl }}/works/">All Works ></a></p>
    </div>
</div>