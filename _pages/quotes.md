---
layout: page
title: quotes
permalink: /quotes/
description: A collection of quotes that I like, if you have suggestions, email me! Currently not working and accepting tips, I have a JSON file with quotes and would like them to appear randomly or all together with images and credit. 
nav: true
nav_order: 6
---

<div class="quotes">
  <ul id="quote-list">
    <!-- Quotes will be added here via JavaScript -->
  </ul>
</div>

<script>
  // Define your quotes as an array of objects directly within JavaScript.
  const quotesList = [
 {
   "Quote": "Be less curious about people and more curious about ideas.",
   "Author": "Maria Sklodowska-Curie (1967-1934)",
   "Image": "https://upload.wikimedia.org/wikipedia/commons/thumb/c/c8/Marie_Curie_c._1920s.jpg/1200px-Marie_Curie_c._1920s.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "To those who can hear me, I say - do not despair. The misery that is now upon us is but the passing of greed - the bitterness of men who fear the way of human progress. The hate of men will pass, and dictators die, and the power they took from the people will return to the people. And so long as men die, liberty will never perish",
   "Author": "Charlie Chaplin (1889-1977), in \"The Great Dictator\"",
   "Image": "https://upload.wikimedia.org/wikipedia/commons/thumb/0/00/Charlie_Chaplin.jpg/640px-Charlie_Chaplin.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "The best theory is inspired by practice. The\nbest practice is inspired by theory.",
   "Author": "Donald Knuth (1938- )",
   "Image": "https://en.wikipedia.org/wiki/File:Donald_Ervin_Knuth_(cropped).jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "A mathematician is a device for\nturning coffee into theorems.",
   "Author": "Alfred Renyi (1921-1970), often ascribed to Paul Erdos (1913-1996)",
   "Image": "https://en.wikipedia.org/wiki/File:Alfred_Kato_Renyi.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "Perhaps even more than to the interaction\nbetween mankind and nature, graph theory is\nbased on the interaction of human beings\nwith each other. ",
   "Author": "Denes Konig (1884-1944)",
   "Image": "https://en.wikipedia.org/wiki/File:Denes_Konig_1928.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "We see the world in terms of our theories. ",
   "Author": "Thomas Kuhn (1922-1996)",
   "Image": "https://en.wikipedia.org/wiki/File:Thomas_Kuhn.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "The unique end of science is the honor of the\nhuman mind.",
   "Author": "Carl Gustav Jacob Jacobi (1804-1851)",
   "Image": "https://it.wikipedia.org/wiki/File:Carl_Jacobi.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "Symmetry, as wide or as narrow as you may\ndefine its meaning, is one idea by which man\nthrough the ages has tried to comprehend and\ncreate order, beauty, and perfection.",
   "Author": "Hermann Weyl (1885-1955)",
   "Image": "https://en.wikipedia.org/wiki/File:Hermann_Weyl_ETH-Bib_Portr_00890.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "The image of the world around us, which we\ncarry in our head, is just a model. Nobody in\nhis head imagines all the world, government or\ncountry. He has only selected concepts, and\nrelationships between them, and uses those to\nrepresent the real system.",
   "Author": "Jay Wright Forrester (1918-2016)",
   "Image": "https://en.wikipedia.org/wiki/File:Jay_Forrester.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "The knowledge of certain principles easily\ncompensates the lack of knowledge of certain\nfacts. ",
   "Author": "Claude Adrien Helvétius (1715-1771)",
   "Image": "https://biografieonline.it/img/bio/c/Claude-Adrien_Helvetius.jpg",
   "Credit": "Biografie Online"
 },
 {
   "Quote": "Probability theory is nothing but common sense reduced to calculation.",
   "Author": "Pierre-Simon Laplace (1749-1827)",
   "Image": "https://en.wikiquote.org/wiki/File:Pierre-Simon_Laplace.jpg",
   "Credit": "Wikiquotes"
 },
 {
   "Quote": "The imaginary numbers are a wonderful flight of God's spirit; they are almost an amphibian between being and not being.",
   "Author": "Gottfried Wilhelm Leibniz (1646-1716)",
   "Image": "https://en.wikipedia.org/wiki/File:Christoph_Bernhard_Francke_-_Bildnis_des_Philosophen_Leibniz_(ca._1695).jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "The law that entropy always increases holds, I think, the supreme position among the laws of Nature. If someone points out to you that your pet theory of the universe is in disagreement with Maxwell's equations - then so much the worse for Maxwell's equations. If it is found to be contradicted by observation - well, these experimentalists do bungle things sometimes. But if your theory is found to be against the Second Law of Thermodynamics I can give you no hope; there is nothing for it to collapse in deepest humiliation.",
   "Author": "Arthur Eddington (1882 – 1944)",
   "Image": "https://en.wikipedia.org/wiki/File:Arthur_Stanley_Eddington.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "My memory for figures, otherwise tolerably accurate, always lets me down\nwhen I am counting beer glasses",
   "Author": "Ludwig Eduard Boltzmann (1844 – 1906)",
   "Image": "https://en.wikipedia.org/wiki/File:Boltzmann2.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "All knowledge is, in final analysis, history.\nAll sciences are, in the abstract, mathematics.\nAll judgements are, in their rationale, statistics.",
   "Author": "Calyampudi Radhakrishna Rao (1920 – 2023)",
   "Image": "https://en.wikipedia.org/wiki/File:Calyampudi_Radhakrishna_Rao_at_ISI_Chennai_(cropped).JPG",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "Mathematics is the most beautiful and most powerful creation of the human spirit.",
   "Author": "Stefan Banach (1892 – 1945)",
   "Image": "https://en.wikipedia.org/wiki/File:Stefan_Banach.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "Something can be more interesting if it is not immediately accepted",
   "Author": "John Nash (1928 – 2015)",
   "Image": "https://en.wikipedia.org/wiki/File:John_Forbes_Nash,_Jr._by_Peter_Badge.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "If one must choose between rigour and meaning, I shall unhesitatingly choose the latter.",
   "Author": "René Frédéric Thom (1923 – 2002)",
   "Image": "https://en.wikipedia.org/wiki/File:Ren%C3%A9_Thom.jpeg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "Bring forward what it true, write it so that it is clear, defend it to your last breath",
   "Author": "Ludwig Eduard Boltzmann (1844 – 1906)",
   "Image": "https://en.wikipedia.org/wiki/File:Boltzmann2.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "Uncertainty is an uncomfortable position. But certainty is an absurd one.",
   "Author": "François-Marie Arouet (1694 – 1778) nom de plume M. de Voltaire",
   "Image": "https://upload.wikimedia.org/wikipedia/commons/thumb/2/2f/Voltaire_-_%C3%89l%C3%A9mens_de_la_philosophie_de_Neuton.png/808px-Voltaire_-_%C3%89l%C3%A9mens_de_la_philosophie_de_Neuton.png",
   "Credit": "Wikipedia"
 }
];

  // Function to populate the list with quotes.
  function populateQuotes() {
    const quoteList = document.getElementById('quote-list');
    
    quotesList.forEach(quote => {
      const listItem = document.createElement('li');
      listItem.innerHTML = `
        <blockquote>${quote.Quote}</blockquote>
        <p class="author">- ${quote.Author}</p>
      `;
      quoteList.appendChild(listItem);
    });
  }

  // Call the function to populate quotes when the page loads.
  window.addEventListener('load', populateQuotes);
</script>
