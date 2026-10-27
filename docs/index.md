---
title: Welcome!
layout: default
use-leaflet: true
---

<section class="flex justify-center">
  <article class="standout-box blue large">
    <div class="big-text header" id="map-box" >
    The Municipal Election <strong>was</strong> October 26, 2026
    </div>

    <p>
    Update, Oct 26: 
    The election is now over. We will publish
    <strong>unofficial</strong> results as
    they become available. You will be able to see the winners in your
    area by searching for your address, just as you did before the
    election.
    </p>

    <div class="content" data-aos="fade-up">
     <p>
     <strong>Type your address to find your candidates, or click your
     location on the map.</strong>
     </p>

     <div class="map-loader" aria-live="polite" data-baseurl="{{ site.baseurl }}">
       <p id="map-loader-status" class="map-loader-status">
         Loading the interactive ward map.
       </p>
     </div>
     {% if site.enable-map-search-nominatim %}
       <div id="map-searchbar"></div>
     {% endif %}

     <div id="map"></div>


     <p>If the map is loading slowly or does
     not load, please use the <a href="/by-ward/">text ward listings</a>.
     </p>
     <p>
     (Note that although the address lookup is
     pretty good, it is not 100% accurate, especially near ward
     boundaries. If in doubt consult your <a href="https://wrvotes.com" 
     target="_blank" class="external">municipality</a>.)
     </p>

    </div> <!-- Data AOS -->

  </article>
</section>

<script defer src="{{ site.baseurl }}/assets/js/home-map-loader.js"></script>
