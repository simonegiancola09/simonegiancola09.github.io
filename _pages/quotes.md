---
layout: page
title: quotes
permalink: /quotes/
description: A collection of quotes that I like, if you have suggestions, email me!
nav: true
nav_order: 5
---

<div id="quote-container">
  <blockquote id="text"></blockquote>
  <p id="author"></p>
  <img id="image">
  <p id="credit"></p>
</div>

<button id="get-random-quote">Get another one</button>

<script>
// JavaScript code to fetch and display random quote with image and credit from your CSV file.
const quotesURL = 'http://simonegiancola09.github.io/assets/csv/quotes_list.csv';

async function getRandomQuote() {
  const response = await fetch(quotesURL);
  const data = await response.text();
  const lines = data.split('\n').filter(Boolean);
  const randomIndex = Math.floor(Math.random() * lines.length);
  const [quote, author, image, credit] = lines[randomIndex].split(',');
  
  document.getElementById('quote').textContent = `"${quote}"`;
  document.getElementById('author').textContent = `- ${author}`;
  document.getElementById('image').src = image;
  document.getElementById('credit').textContent = `Image Credit: ${credit}`;
}
window.addEventListener('load', getRandomQuote);

//document.getElementById('get-random-quote').addEventListener('click', getRandomQuote);
</script>

