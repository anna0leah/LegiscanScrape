# LegiscanScrape
This is an attempt to scrape Legiscan bills related to "Unborn * Dignity"

It's been a long, strange trip with two major hang-ups:
1) Search results were limited by term, for reasons I need addressed by the company itself (and only figured out after they could respond to me. They're great).
2) I didn't run through the different search keyphrases listed at the top.

The goal of this scrape is to look through Legiscan, a database of proposed state legislations. 
The site often breaks the information into searches by state and term.

We wanted to answer the question: where, when, by whom, and to what level of success has legislation been floated that uses the keyphrases in question.
Ideally, we could examine the differences between those keyphrases, which were recommended to us by a legal expert as indicative of a political ideology split happening in statehouses.

A free account allows users to search by keyphrases across states and terms (meaning years the legislatures are present).
However, the API searches does not allow for this flexibility of searches. Neither does entering the URL without signing in.
So, this scrape only searches all states but not all terms.

Beyond these limitations, the scrape was fairly straightforward:
1) using the provided API, pull down bill information based on keyphrase
2) iterate through pages
3) clean the data and enter it into a usable dataframe

If I were able to iterate through all the keyphrases and terms, I would have loved to provide a data-based assessement of these ideologies at play in capitols across the country.
Maybe one day, for my upcoming capstone from CUNY's Craig Newmark School of Journalism...

You can find your own dataset for free by signing up for an API at https://legiscan.com/legiscan.
