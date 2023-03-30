# ArXiV_Summary
Collaboration with Jesse Parrish, Vlad Kovalchuk, and Xiao Zhuang at the University of Denver. Weekly newsletter providing bullet point summaries of a selection of recently posted papers on arXiv.

Project Outline

Python file (app.py) will use BeautifulSoup to parse arXiv.org with the relevant tags for papers posted in the previous week
  - Starting with cs.LG (ML), stat (statistics), q-fin (quant finance), math, astro-ph (astrophysics)

GPT Processing
For each category: 
  - Extract all titles and send to GPT to ask what the most impactful (20) papers are. 
    -  This step is to limit the amount of GPT processing for categories that have numerous papers
  - Of those (20), ask GPT to summarize the abstract in 1-3 bullet points
  - From those bullet points, have GPT select and rank the most impactful (5)

Newsletter Creation
For each category: 
  - Create a string that has in descending order the title of the paper wrapped in a hyperlink followed by the bullet point summary
  - Send string out in email as a newsletter


Misc Notes
Querying arXiv: https://info.arxiv.org/help/api/basics.html
