---
layout: page
title: quotes
permalink: /quotes/
description: A collection of quotes that I like. If you have suggestions, email me!
nav: false
nav_order: 6
---

<div class="quotes" style="text-align:center; max-width:700px; margin:0 auto;">
  <div id="quote-display" style="margin-top:2rem;">
    <!-- Random quote will appear here -->
  </div>
  <button onclick="showRandomQuote()" class="btn btn-outline-primary" style="margin-top:1.5rem;">
    🎲 New Quote
  </button>
</div>

<script>
  let quotesList = [];
  let lastIndex = -1;

  function showRandomQuote() {
    if (quotesList.length === 0) return;

    let index;
    do {
      index = Math.floor(Math.random() * quotesList.length);
    } while (index === lastIndex && quotesList.length > 1);
    lastIndex = index;

    const quote = quotesList[index];
    const display = document.getElementById('quote-display');

    const hasImage = quote.Image && quote.Image.trim() !== '';

    display.innerHTML = `
      <blockquote style="font-size:1.3rem; font-style:italic;">${quote.Quote}</blockquote>
      <p class="author" style="margin-top:1rem;">— ${quote.Author}</p>
      ${hasImage ? `
        <div id="quote-image-block" style="margin-top:1rem;">
          <img id="quote-img" src="${quote.Image}" alt="${quote.Author}"
               style="height:80px; border-radius:50%; object-fit:cover; vertical-align:middle; margin-right:8px;">
          <em>Image credit: ${quote.Credit}</em>
        </div>
      ` : ''}
    `;

    if (hasImage) {
      const img = document.getElementById('quote-img');
      img.onerror = function () {
        document.getElementById('quote-image-block').style.display = 'none';
      };
    }
  }

  window.addEventListener('load', () => {
    fetch('{{ "/assets/json/quotes.json" | relative_url }}')
      .then(res => res.json())
      .then(data => {
        quotesList = data;
        showRandomQuote();
      })
      .catch(err => {
        document.getElementById('quote-display').innerHTML =
          '<p>Could not load quotes right now.</p>';
        console.error('Failed to load quotes:', err);
      });
  });
</script>