# NLP-CDST
_Natural Language Processing Clinical Decision Support Tool_

This repo holds the code associated with a research paper that I am writing. Updates to follow.

## Version 1

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
