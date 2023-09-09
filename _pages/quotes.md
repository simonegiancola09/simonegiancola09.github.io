---
layout: page
title: quotes
permalink: /quotes/
description: A collection of quotes that I like, if you have suggestions, email me! Currently need to adjust some comma vs CSV issues.
nav: true
nav_order: 5
---

<div id="quote-container">
  <blockquote id="Quote"></blockquote>
  <p id="Author"></p>
  <img id="Image">
  <p id="Credit"></p>
</div>

<button id="get-random-quote">Get another one</button>

<script>
// JavaScript code to fetch and display random quote with image and credit from your CSV file.
const quotesURL = 'https://raw.githubusercontent.com/simonegiancola09/simonegiancola09.github.io/master/assets/json/quotes_list.json';

async function getRandomQuote() {
  const response = await fetch(quotesURL);
  const data = await response.text();
  const lines = data.split('\n').filter(Boolean);
  const randomIndex = Math.floor(Math.random() * lines.length);
  const [Quote, Author, Image, Credit] = lines[randomIndex].split(',');
  
  document.getElementById('Quote').textContent = `"${Quote}"`;
  document.getElementById('Author').textContent = `- ${Author}`;
  document.getElementById('Image').src = Image;
  document.getElementById('Credit').textContent = `Image Credit: ${Credit}`;
}
window.addEventListener('load', getRandomQuote);

//document.getElementById('get-random-quote').addEventListener('click', getRandomQuote);
</script>

