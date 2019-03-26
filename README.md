# News_Clasifier
Gather news from multiple sites of information and classifies them.
The posts folder has multiple posts from multiple sites.
The evaluations folder has each post from each category evaluated how much does it belong to each category.

Every post is in JSON format.
The "evaluation" is quite simple:
 1) tokenize the words from the post's title and description with nltk.
 2) for each noun found the program tries to calsify it to each certain category and find the similarity using GoogleNews-vectors-negative300.
 3) adds all the scores into result dictionary.
