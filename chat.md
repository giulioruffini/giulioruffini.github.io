---
layout: default
title: Papers Chat
permalink: /chat/
---

# Chat with my papers

Type a query below to search and get answers grounded in my paper collection.

<!-- Widget JavaScript bundle -->
<script src="https://cloud.google.com/ai/gen-app-builder/client?hl=en_US"></script>

<!-- Search widget element is not visible by default -->
<gen-search-widget
  configId="65c0645c-a58e-4f55-8924-f1d22a0fa5b8"
  location="global"
  triggerId="searchWidgetTrigger">
</gen-search-widget>

<!-- Element that opens the widget on click. It does not have to be an input -->
<input placeholder="Search here" id="searchWidgetTrigger" style="width: 100%; max-width: 520px; padding: 12px; font-size: 16px;" />