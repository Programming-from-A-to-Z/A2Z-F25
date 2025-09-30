# Language Models

## [Language Model slides](https://docs.google.com/presentation/d/1M8zwy7yKA7G6EzSYS8qnYRNuQ8KJkoo-M5YG6OM4vKk/edit?usp=sharing)

## Weighted Selection / Sampling

- 💻 [Weighted Selection p5.js example](https://editor.p5js.org/a2zitp/sketches/_NgAEnEjZ) (with temperature!)
- 🚂 [Weighted Selection Algorithm video](https://youtu.be/ETphJASzYes)
- 📚 [Nature of Code Genetic Algorithm Section on Weighted Sampling](https://natureofcode.com/genetic-algorithms/#step-2-selection-1)
- 📚 [How to Generate Text Hugging Face blog post](https://huggingface.co/blog/how-to-generate) (covers temperature, top_p, and top_k)

## Markov Chains

- 📕 [Markov Chains](http://setosa.io/blog/2014/07/26/markov-chains/) by Victor Powell and Lewis Lehe
- 🚨 [Markov Chain Coding Challenge](https://thecodingtrain.com/challenges/42-markov-chain-name-generator)
- 💻 [Markov Chain p5.js code examples](https://editor.p5js.org/a2zitp/collections/WEXEPRHuE), [quick note about `getURLParams()`](https://github.com/Programming-from-A-to-Z/A2Z-F23/wiki/Using-URL-Query-String)
- 💻 [Markov Chain node.js example](https://github.com/Programming-from-A-to-Z/Markov-Node)
- 💻 [Markov Chain Discord Bot example](https://github.com/Programming-from-A-to-Z/Markov-Discord-Bot)
- 📚 [N-Grams and Markov Chains by Allison Parrish](http://www.decontextualize.com/teaching/rwet/n-grams-and-markov-chains/)
- 📚 [2016 Markov Chains notes from A2Z](https://shiffman-archive.netlify.app/a2z/markov/)

### Markov Project References

- 🎨 [ITP Course Generator by Allison Parrish](http://static.decontextualize.com/toys/next_semester)
- 🎨 [Markov Visualizer](https://x.com/tylerangert/status/1385677572185407489) by Tyler Angert
- 🎨 [WebTrigrams by Chris Harrison](http://www.chrisharrison.net/index.php/Visualizations/WebTrigrams)
- 📈 [Google N-Gram Viewer](https://books.google.com/ngrams), [google blog post about n-grams](http://googleresearch.blogspot.com/2006/08/all-our-n-gram-are-belong-to-you.html)
- 🎨 [King James Programming](http://kingjamesprogramming.tumblr.com/)
- 🎨 [Gnoetry](http://www.beardofbees.com/gnoetry.html)

## Context-Free Grammars

- 🚨 [CFG with Tracery](https://youtu.be/C3EwsSNJeOE?list=PLRqwX-V7Uu6YrbSJBg32eTzUU50E2B8Ch), [Tracery by Kate Compton](http://tracery.io/)
- 📕 [Tracery: An Author-Focused Generative Text Tool](https://www.researchgate.net/profile/Quinn_Kybartas/publication/300137911_Tracery_An_Author-Focused_Generative_Text_Tool/links/5ed3c8c14585152945220c14/Tracery-An-Author-Focused-Generative-Text-Tool.pdf)
- 📚 [Context-Free Grammars by Allison Parrish](http://www.decontextualize.com/teaching/rwet/recursion-and-context-free-grammars/)
- 🍿 [CFG Coding Challenge "from scratch" with p5.js](https://thecodingtrain.com/challenges/43-context-free-grammar)
- 🍿 Additional: [Intro to CFG](https://youtu.be/Rhqk9HYiB7Q), [CFG with RiTa](https://youtu.be/VaAoIaZ3YKs)
- 💻 [CFG p5.js code examples](https://editor.p5js.org/a2zitp/collections/5IFiJuQZa)
- 💻 [RiGrammer](https://rednoise.org/rita/reference/RiTa/grammar/index.html) from RiTa library, [RiGrammar example](https://editor.p5js.org/rita-examples/sketches/7vWYB1HEn)
- 📚 [2016 Notes on Context-Free Grammar](https://shiffman-archive.netlify.app/a2z/cfg/)

### CFG Project References

- [Art Assignment Bot](https://twitter.com/artassignbot?lang=en)
- [Monstr (a dating website, but for monsters)](http://www.plusultra.ninja/monstr.html)
- [What color is this dress?](http://www.galaxykate.com/dress/)
- [Happy Valentine's Day](http://www.galaxykate.com/apps//vday/vday.html?s=HEJ8)
- [SCIgen - An Automatic CS Paper Generator](https://pdos.csail.mit.edu/archive/scigen/) -- _no longer working_ 😢

### CFG Visual Art

- 📚 [Algorithmic Beauty of Plants](http://algorithmicbotany.org/papers/abop/abop.pdf)
- 🍿 [L-System Coding Challenge Video](https://thecodingtrain.com/challenges/16-l-system-fractal-trees)

## Transformer Language Models

_(We're going to cover more about LLMs and AI in future weeks, but here we'll just dip our toe in the water and test LLMs in JS to compare and contrast with markov chains and grammars)_

### Transformers.js

- 💻 [p5.js LLM examples](https://editor.p5js.org/a2zitp/collections/Y1oZ1As1s)
- [SmolLM 3](https://github.com/huggingface/smollm)
- [WebAI Summit Transformers.js Slides](https://docs.google.com/presentation/d/1FTKmN9ZWyrBjQyp6-osPyvLzKiXqjqCSZvb0-FIqme0/edit?usp=sharing) - Thank you @xenova!
- [Transformers.js Documentation](https://huggingface.co/docs/transformers.js/)
- [Transformers.js v3: WebGPU Support, New Models & Tasks, and More…](https://huggingface.co/blog/transformersjs-v3)
- [Ollama](https://ollama.com/)

## Assignment

- Read [Language models can only write ransom notes](https://posts.decontextualize.com/language-models-ransom-notes/) by Allison Parrish

Choose one (or more!) of the following approaches to explore computational text generation. As you experiment, consider Parrish's discussion of "cuts" in collage, the difference between "collections" and "hoards," and how different computational methods make visible (or obscure) their source materials and processes.

_(It is not required to write any new code for this assignment. You are welcome to run one or more of the provided examples with your own data. You can document the results in a blog post (or link to a web page where the text is generated). I'll include some other ideas below in case you are feeling ambitious.)_

### Markov Chains

Use one of the [existing examples](https://editor.p5js.org/a2zitp/collections/WEXEPRHuE) to generate text with your own input data. Experiment with the "order" and "maximum" length variables. Try mixing multiple texts. Copy paste your favorite outputs from the browser and document in a blog post.

It is not required to write any new code for this assignment, however I'll include some ideas for further exploration below.

- Design a webpage that displays the output of a markov generator a la [Allison Parrish's ITP course creator](http://static.decontextualize.com/toys/next_semester).
- Create a bot that generates its output based on a markov chain.
- Use a markov chain on something other than text. Record your own sequence of daily habits. Try musical notes. Could colors or shapes be generated with a markov chain? What else? You can find examples for [musical markov chains](https://luisaph.github.io/the-code-of-music-2018/#Markov) from Luisa Pereira's [Code of Music materials](https://luisaph.github.io/the-code-of-music-2018/).
- Thinking back to [the word counting material](https://github.com/shiffman/A2Z-F25/tree/main/02-word-counting), visualize n-gram frequencies and/or markov probabilities.

### Context-Free Grammars

Invent your own grammar and generate text. You can use [Tracery](http://tracery.io/), [any of my examples](https://editor.p5js.org/a2zitp/collections/5IFiJuQZa), or try [RiGrammer](https://rednoise.org/rita/reference/RiTa/grammar/index.html) from the RiTa library.

Getting results from a context-free-grammar can be tricky. Short and sweet, highly structured ideas tend to work well. For example.

- A coffee drink order generator.
- An apology generator.
- An ITP project idea generator.
- A knock knock joke generator.

Something you might consider is pulling the "terminal" words for your grammar from an API or other data source. You are also welcome to explore generative visual art basing your exercise off of the L-System material described above. Or what else can you generate from a Context-Free Grammar? Music?

### Large Language Models (LLMs)

Experiment with running a small language model locally in the browser using [transformers.js](https://huggingface.co/docs/transformers.js/) and [SmolLM 3](https://github.com/huggingface/smollm). Consider how this approach compares to Markov chains and context-free grammars in terms of Parrish's concepts of "cuts," materiality, and the visibility of source materials.

### Add your assignment below via Pull Request

_(Please note you are welcome to post under a pseudonym and/or password protect your published assignment. For NYU blogs, privacy options are covered in the [NYU Wordpress Knowledge Base](https://wp.nyu.edu/knowledge/). Finally, if you prefer not to post your assignment at all here, you may email the submission.)_

- Name - [post title](post url)
- Haya - [Excuses](https://www.notion.so/Excuses-27dc09edca17800699afd5e96e371ad2)
- Niki - [Week 4 Assignment Fortune Sphere&Lucky Message](https://reinvented-spoonbill-0fb.notion.site/A-to-Z-Week-4-Language-Model-Niki-27d0470c67d480439fc0d4e6cd7aac56)
- Billy - [My Vampire Chatbot] (https://billybil30itpday.notion.site/Computational-Text-Week-4-27eedbdaee0280ad88bad5a8a0ef449b?source=copy_link)
- Ping - [Horror Recipe](https://www.notion.so/pinglin36/Week4-Markov-277e2a20970580eb9101ecaf05530647?source=copy_link)
- Fiona - [Week 4 Secret Rizz Up Lines Website](https://www.notion.so/Fiona-s-Assignment-4-Language-Models-27c701873e0780b79baff7d55310ace0?source=copy_link) 
- Junqi - [Test Projects related to Cultural Topics](https://fuzzy-mask-71e.notion.site/COMPUTATIONAL-TEXT-A-Z-262480e9e232806f96c3f65ab685c294?source=copy_link)
- rachel - [Markov font](https://rachel-shin-itp.notion.site/week-5-267d9b4cf2a680bb98e1f4e7b3260aca?source=copy_link)

## Emoji Key for Video Tutorials, Readings, and more

- 🚨 Watch this video tutorial! (this is technical info needed for the examples). Of course if you alreaddy know this material, you can skip.
- 🔢 This is found in a group, maybe pick just one to check out!
- 🍿 Additional video if you have a particular interest and want to do a deeper dive.
- 📕 Required reading! Let's make sure we all have read this.
- 📚 Optional additional reading for a deeper dive.
- 💻 Code examples here!
- 📈 Class presentation slides
- 🔗 Extra reference material / link
