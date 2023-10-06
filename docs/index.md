---
layout: default
title: Home
---


<section class="hero">
	<div class="small-container">
		<h2>新鲜，即时，当地，当季</h2>
		<p class="sub-text">大洋<strong>瑞福</strong> 是您寻找的新鲜海鲜的极佳选择，以品质和可靠性为您的餐桌带来诱人的海鲜美味。</p>
	</div>
</section>

<div class="container">
	<p class="post-hero center-text spacing"></p>
</div>



<div class="container">
  {% assign top_products = site.top_products%}
  {% for top_product in top_products %}
    <div class="columns spacing">
      <a href="{{ top_product.recipe_url }}">
        <img class="div-img column half" src="{{ top_product.image_path }}" alt="{{ top_product.title}}"/>
        <div class="column half">
          <h3>{{ top_product.title }}</h3>
          <p>{{ top_product.description }}</p>
          <p style="color:tomato;">点击了解产品细节</p>
        </div>
      </a>
    </div>
  {% endfor %}
</div>