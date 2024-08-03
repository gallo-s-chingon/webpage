---
layout: single
title: Contact Us
sitemap: true
permalink: /outreach
header:
  overlay_filter: "0.6"
  overlay_image: "/images/bbreno.png"
excerpt: "testing words ipsom lorem"layout: default
---

<h1>Contact Us</h1>

<p>Please select your category:</p>

<select id="categorySelect">
  <option value="">Choose an option</option>
  <option value="band">Band/Artist</option>
  <option value="promoter">Promoter</option>
  <option value="fan">Music Fan</option>
  <option value="vendor">Vendor</option>
---
layout: single
title: Contact Us
sitemap: true
permalink: /outreach
header:
  overlay_filter: "0.6"
  overlay_image: "/images/bbreno.png"
excerpt: "testing words ipsom lorem"
---

<h1>Contact Us</h1>

<p>Please select your category:</p>

<select id="categorySelect">
  <option value="band">Band/Artist</option>
  <option value="promoter">Promoter</option>
  <option value="fan">Music Fan</option>
  <option value="vendor">Vendor</option>
  <option value="general">General Inquiry</option>
</select>

<div id="linkContainer" style="display: none; margin-top: 20px;">
  <a id="formLink" href="#" target="_blank">Click here to fill out the form</a>
</div>

<script>
  const categorySelect = document.getElementById('categorySelect');
  const linkContainer = document.getElementById('linkContainer');
  const formLink = document.getElementById('formLink');

  const formUrls = {
    band: 'https://docs.google.com/forms/d/1mez8avQfWKgSt_HaSd9YiHfrchpCSFlZryGMMwOp35o',
    promoter: 'https://docs.google.com/forms/d/1q0xLpLmynwTLBNzlEx2sTTlasha5Bz3aPlQq0CUeeXM',
    fan: 'https://docs.google.com/forms/d/1OESAeo1VlJrYJ0fC-e3wA-yRQ_qpYtdc9frYbnBQIoY',
    vendor: 'https://docs.google.com/forms/d/1DdP8vDLUo1_gPeT0-pwcs8vV-YFcvTbY3aCO84JXTsg'
    general: 'https://docs.google.com/forms/d/1OESAeo1VlJrYJ0fC-e3wA-yRQ_qpYtdc9frYbnBQIoY'
  };

  categorySelect.addEventListener('change', function() {
    const selectedCategory = this.value;
    if (selectedCategory) {
      formLink.href = formUrls[selectedCategory];
      linkContainer.style.display = 'block';
    } else {
      linkContainer.style.display = 'none';
    }
  });
</script>
