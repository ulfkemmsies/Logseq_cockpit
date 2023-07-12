- # Make Logseq QA Flashcards
    prompt-template:: Make Logseq Flashcards
	- ```prompt
	  You are now an expert on Micropropulsion and are helping me review for my exam on this topic.
	  I want you to create a deck of flashcards from the text.
	  
	  Instructions to create a deck of flashcards:
	  - Keep the flashcards simple, clear, and focused on the most important information.
	  - Make sure the questions are specific and unambiguous.
	  - Use simple and direct language to make the cards easy to read and understand.
	  - Answers should contain only a single key fact/name/concept/term.
	  - If the text has nested bullet points, be sure to consider all the text inside each bullet.
	  
	  Let's do it step by step when creating a deck of flashcards:
	  1. Rewrite the content using clear and concise language while retaining its original meaning.
	  2. Split the rewritten content into several sections, with each section focusing on one main point.
	  3. Utilize the sections to generate multiple flashcards, and for sections with more than 10 words, split and summarize them before creating the flashcards.
	  4. Format them like this:
	  
	  Question: What is the third planet from Earth?
	  Answer: Earth.
	  
	  Do not write the name of the text. Do not write "flashcard". Do not number them.
	  
	  Text to consider follows:
	  ```
- # Make Logseq Cloze Flashcards
    prompt-template:: Make Logseq Cloze Flashcards
	- id:: d9412ea5-610c-4c98-a252-10605cc0d391
	  ```prompt
	  Make cloze flashcards from the text and be sure to make the questions as atomic as possible. Cover all the content in the text. Here is an example for formatting:
	  Original text: Earth is the third planet from the Sun and is the only planet in the Solar System with life.
	  Soem possible flashcards:
	  {{cloze Earth}} is the third planet from the Sun and is the only planet in the Solar System with {{cloze life}}.
	  The third planet from the Sun, {{cloze Earth}}, is known for {{cloze having life on it}}.
	  ```