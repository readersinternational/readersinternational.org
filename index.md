---
layout: default
---

<section>
  <div class="js-Carousel" id="carousel">
    <ul>
    {% assign books = site.books | where:"in_carousel","true" %}
    {% for book in books %}
      <li style="background-image: url({{ book.cover }}); background-position: center {{ book.carousel_y }};">
        <a href="{{ book.permalink }}">
          <div class="carousel-title">{{ book.title }}</div>
        </a>
      </li>
    {% endfor %}
    </ul>
  </div>
</section>
<br><br>
[View all of our books](/books)
<br><br>
# Our Mission and Values

The mission of Readers International remains the same as it was at the start: to bring to readers the best international literature, especially by authors representing the national conscience of their countries, who are therefore often subject to political pressures, censorship and exile.
<br><br>
[Read More](/about-contact)