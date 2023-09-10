---
layout: page
title: quotes
permalink: /quotes/
description: A collection of quotes that I like, if you have suggestions, email me! Refresh the page and a new one will appear. 
nav: true
nav_order: 5
---

<div id="quote-container">
  <blockquote id="Quote"></blockquote>
  <p id="Author"></p>
</div>


<script>
// JavaScript code to fetch and display random quote with image and credit from your CSV file.
const quotesURL = 'https://raw.githubusercontent.com/simonegiancola09/simonegiancola09.github.io/master/assets/json/quotes_list.json';

async function getRandomQuote() {
  try {
    const response = await fetch(quotesURL);
    const data = await response.json();
    const randomIndex = Math.floor(Math.random() * data.length);
    const { Quote, Author, Image, Credit } = data[randomIndex];

    document.getElementById('Quote').textContent = Quote;
    document.getElementById('Author').textContent = `- ${Author}`;
    //document.getElementById('Image').src = Image;
    //document.getElementById('Credit').textContent = `Image Credit: ${Credit}`;
  } catch (error) {
    console.error('Error fetching or parsing JSON data:', error);
  }
}
window.addEventListener('load', getRandomQuote);

//document.getElementById('get-random-quote').addEventListener('click', getRandomQuote);
</script>

