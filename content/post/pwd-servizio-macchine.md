+++
author = "DS"
categories = ["tips", "prodotti", "CAT"]
date = 0001-01-01T00:00:00Z
description = ""
draft = false
slug = "pwd-servizio-macchine"
tags = ["tips", "prodotti", "CAT"]
title = "Pwd servizio macchine"

+++


<!-- Everything inside of #tag pulls data from the tag -->
{{#tag}}
  <header>
  	{{#if feature_image}}
    	<img src="{{feature_image}}" alt="{{name}}" />
    {{/if}}
  </header>

  <section class="author-profile">
  	<h1>{{name}}</h1>
    {{#if description}}
      <h2>{{description}}</h2>
    {{/if}}
  </section>
{{/tag}}

<main role="main">
    <!-- includes the post loop - partials/loop.hbs -->
    {{> "loop"}}
</main>

<!-- Previous/next page links - displayed on every page -->
{{pagination}}



