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
    {"Quote":"Dubium sapientiae initium",
"Author":"René Descartes (1596-1650)",
"Image": "https://it.wikipedia.org/wiki/File:Frans_Hals_-_Portret_van_Ren%C3%A9_Descartes.jpg",
   "Credit": "Wikipedia"
}, 
    {"Quote":"Se hai 5 lire compra 5 lire di fiducia in te stesso. Persevera nelle decisioni prese. Credo solo ai fatti provati.",
"Author":"Nella targa regalata a Eugenio Cefis dopo avere svolto il praticantato (ref. Paolo Morando: Eugenio Cefis, una storia italiana di potere e misteri)",
"Image": "https://www.laterza.it/immagini/copertine-big/9788858143872.jpg",
   "Credit": "Editori Laterza"
},
    {"Quote":"One day, in retrospect, the years of struggle will strike you as the most beautiful.",
"Author":"Sigmund Freud (1856–1939)",
"Image": "https://en.wikipedia.org/wiki/File:Sigmund_Freud,_by_Max_Halberstadt_(cropped).jpg",
   "Credit": "Wikipedia"
},
{"Quote":"The first principle is that you must not fool yourself — and you are the easiest person to fool.",
"Author":"Richard Feynman (1918-1988)",
"Image": "https://en.wikipedia.org/wiki/File:Richard_Feynman_Nobel.jpg",
   "Credit": "Wikipedia"
},
{"Quote":"One has an ideology when ideas are absent. ",
"Author":"I do not remember where I heard this but like it a lot.",
"Image": "https://images.twinkl.co.uk/tw1n/image/private/t_630/u/ux/question-mark_ver_1.jpg",
   "Credit": "Twinkl"
},
{"Quote":"A generating function is a clothesline on which we hang up a sequence of numbers for display.",
"Author":"Herbert Saul Wilf (1931-2012)",
"Image": "https://en.wikipedia.org/wiki/File:Herbert_Wilf.jpg",
   "Credit": "Wikipedia"
},
{"Quote":"Physics is a dialectical learning process, it is not constructive.",
"Author":"Daniel Schroeder [The Cartesian Cafe podcast]",
"Image": "https://www.weber.edu/wsuimages/physics/faculty/Dan-Schroeder-3599-for-web.jpg",
   "Credit": "Weber State University"
},
{"Quote":"I thought fit to write out for you and explain in detail in the same book the peculiarity of a certain method, by which it will be possible for you to get a start to enable you to investigate some of the problems in mathematics by means of mechanics. [. . . ] it is of course easier, when we have previously acquired, by the method, some knowledge of the questions, to supply the proof than it is to find it without any previous knowledge.",
 "Author": "Archimedes [from The Method] 3rd Century BC",
 "Image": "https://en.wikipedia.org/wiki/File:Domenico-Fetti_Archimedes_1620.jpg",
   "Credit": "Wikipedia"
},
    {
   "Quote": "The purpose of computing is insight, not numbers.",
   "Author": "Richard Hamming (1915 - 1998)",
   "Image": "https://upload.wikimedia.org/wikipedia/en/0/08/Richard_Hamming.jpg",
   "Credit": "Wikipedia"
 },
  {
   "Quote": "Mathematics is a language",
   "Author": "Josiah Willard Gibbs (1839-1903)",
   "Image": "https://upload.wikimedia.org/wikipedia/commons/thumb/c/c7/Josiah_Willard_Gibbs_-from_MMS-.jpg/440px-Josiah_Willard_Gibbs_-from_MMS-.jpg",
   "Credit": "Wikipedia"
 },
  {
   "Quote": "Shut up and calculate",
   "Author": "Nathaniel David Mermin (1935-)",
   "Image": "https://upload.wikimedia.org/wikipedia/commons/thumb/a/ac/Mermin_Stockholm_2009.jpg/600px-Mermin_Stockholm_2009.jpg",
   "Credit": "Wikipedia"
 },
  {
   "Quote": "I believe that mathematical reality lies outside us, that our function is to discover or observe it, and that the theorems which we prove, and which we describe grandiloquently as our ``creations'', are simply our notes of our observations. This view has been held, in one form or another, by many philosophers of high reputation from Plato onwards, and I shall use the language which is natural to a man who holds it.",
   "Author": "Godfrey Harold Hardy (1877-1947)",
   "Image": "https://upload.wikimedia.org/wikipedia/commons/3/35/Ghhardy%4072.jpg",
   "Credit": "Wikipedia"
 },
{
   "Quote": "Before I came here I was confused about this subject. Having listened to your lecture I am still confused. But on a higher level.",
   "Author": "Enrico Fermi (1901-1954)",
   "Image": "https://tr.wikipedia.org/wiki/Dosya:Enrico_Fermi_1943-49.jpg",
   "Credit": "Wikipedia"
 },

 {
   "Quote": "Be less curious about people and more curious about ideas.",
   "Author": "Maria Sklodowska-Curie (1967-1934)",
   "Image": "https://upload.wikimedia.org/wikipedia/commons/thumb/c/c8/Marie_Curie_c._1920s.jpg/1200px-Marie_Curie_c._1920s.jpg",
   "Credit": "Wikipedia"
 },
 {
   "Quote": "To those who can hear me, I say - do not despair. The misery that is now upon us is but the passing of greed - the bitterness of men who fear the way of human progress. The hate of men will pass, and dictators die, and the power they took from the people will return to the people. And so long as men die, liberty will never perish. \n Soldiers! don’t give yourselves to brutes - men who despise you - enslave you - who regiment your lives - tell you what to do - what to think and what to feel! Who drill you - diet you - treat you like cattle, use you as cannon fodder. Don’t give yourselves to these unnatural men - machine men with machine minds and machine hearts! You are not machines! You are not cattle! You are men! You have the love of humanity in your hearts! You don’t hate! Only the unloved hate - the unloved and the unnatural! Soldiers! Don’t fight for slavery! Fight for liberty! \n In the 17th Chapter of St Luke it is written: “the Kingdom of God is within man” - not one man nor a group of men, but in all men! In you! You, the people have the power - the power to create machines. The power to create happiness! You, the people, have the power to make this life free and beautiful, to make this life a wonderful adventure. \n Then - in the name of democracy - let us use that power - let us all unite. Let us fight for a new world - a decent world that will give men a chance to work - that will give youth a future and old age a security. By the promise of these things, brutes have risen to power. But they lie! They do not fulfil that promise. They never will! \n Dictators free themselves but they enslave the people! Now let us fight to fulfil that promise! Let us fight to free the world - to do away with national barriers - to do away with greed, with hate and intolerance. Let us fight for a world of reason, a world where science and progress will lead to all men’s happiness. Soldiers! in the name of democracy, let us all unite!",
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
