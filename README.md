# NLP-CDST
_Natural Language Processing Clinical Decision Support Tool_

This repo holds the code associated with [this research paper that I am writing](https://drive.google.com/file/d/1KsSOd4oMXm7gWdZcjIgTl9msBGE--E8l/view?usp=share_link). Updates to follow.

# Background:
### From the paper:
>This paper explores a potential application of machine learning (ML) in mental and behavioral healthcare. While some research has been published in this area, there is room for new or expanded applications of this technology in various clinical settings. In a comprehensive 2019 review entitled *[Machine learning in mental health: a scoping review of methods and applications](https://doi.org/10.1017/S0033291719000151)*, Shatte et al. concluded, “Overall, it is clear that ML can significantly improve the detection and diagnosis of mental health conditions…However, this work is currently limited and further research is required to identify additional benefits of ML to these areas (Shatte et al., 2019).

>Our tool is intended to assist clinicians in identifying adolescent patients at risk for depression in a primary care setting. The creation of this tool was guided by the recommendations of the American Academy of Pediatrics, as outlined in their 2018 review entitled, *[Guidelines for Adolescent Depression in Primary Care (GLAD-PC)](https://publications.aap.org/pediatrics/article/141/3/e20174081/37626/Guidelines-for-Adolescent-Depression-in-Primary)*  (Zuckerbrot et al., 2018).


# Versioning:
## Version 1 (11/28/22)

Nothing to note.

## Version 2 (11/30/22)

### Changes

- Updated get_response function to include choice of model
- Refactored some functions
- Query embedding is now based on a summary of the case note, which is via get_response
- Sliced text_and_embeddings to include only the first 727 items
- Created a cell to see the top 10 most relevant embeddings

### BUGS

- It doesn't work from start to finish becasue of some global variables/arguments issues. Big problem.

## Version 3

### Planned Changes

- Refactor to work from start to finish
- Aggregate various arguments into one standard class object
- Modify run_tool function to take one JSON object as a request and return one JSON object as a response, to prep for potential API creation

# References

Rachel A. Zuckerbrot, Amy Cheung, Peter S. Jensen, Ruth E.K. Stein, Danielle Laraque, GLAD-PC STEERING GROUP, Anthony Levitt, Boris Birmaher, John Campo, Greg Clarke, Graham Emslie, Miriam Kaufman, Kelly J. Kelleher, Stanley Kutcher, Michael Malus, Diane Sacks, Bruce Waslick, Barry Sarvet; Guidelines for Adolescent Depression in Primary Care (GLAD-PC): Part I. Practice Preparation, Identification, Assessment, and Initial Management. Pediatrics March 2018; 141 (3): e20174081. 10.1542/peds.2017-4081

Shatte, A. B. R., Hutchinson, D. M., & Teague, S. J. (2019). Machine learning in mental health: a scoping review of methods and applications. Psychological medicine, 49(9), 1426–1448. https://doi.org/10.1017/S0033291719000151

