---
layout: default
title: Papers Chat
permalink: /chat/
---

# Chat with my KT papers

Type a query below to search and get answers grounded in my paper collection.

<!-- Widget JavaScript bundle -->
<script src="https://cloud.google.com/ai/gen-app-builder/client?hl=en_US"></script>

<!-- Search widget element is not visible by default -->
<gen-search-widget
  configId="6164134b-bf20-4d5b-9f1b-fa12cabab8c9"
  location="eu"
  triggerId="searchWidgetTrigger">
</gen-search-widget>

<!-- Element that opens the widget on click. It does not have to be an input -->
<input placeholder="Search here" id="searchWidgetTrigger" />