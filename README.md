# spelling-rules
A project with the goal of identifying and teaching statistically-derived spelling rules for English words

Pre-processing/data cleaning:
1) Extact word, etymology, and definition from ProjectGutenberg Webster's Unabridged Dictionary
2) Store data fields in CSV/DataFrame format

Part 1: Extracting Rules
3) Identify n-character patterns (n-grams) and their rate of occurrence in:
      a) The entire dataset
      b) Subsets of the main dataset (partitioned by language(s) of origin)
4) Test whether the n-grams appear more frequently within subsets than the overall population
5) Summarize findings (e.g. string "schw" appears 400% more commonly in words with German origin than other words)

Part 2: User Engagement
6) Write module which contains functions for helping the user test/implicitly learn:
      a) Etymologies
      b) Definitions
      c) Their knowledge of the above
      
Section A: Self-discovery/testing on spelling rules (word-origin pairings)
7) Write function to:
      a) Randomly pull 1 word/language of origin and display, asking which language of origin/word fits what's displayed
      b) Present user with 4 options of language of origin/word
      c) Ask user to input which option is correct
      d) Evaluate and store whether user is correct/incorrect for that word
      e) If correct: tell user they were correct; If incorrect: tell user they were incorrect and show which answer was correct
      f) Call the function again OR end
8) When user done, state number instances encountered and % correct overall and by language of origin (call out top/bottom few)

Section B: Self-discovery/testing on word-definition pairings
9) Write function to:
      a) Randomly pull 1 word/definition and display, asking which definition/word fits what's displayed
      b) Present user with 4 options of definition/word
      c) Ask user to input which option is correct
      d) Evaluate and store whether user is correct/incorrect for that word
      e) If correct: tell user they were correct; If incorrect: tell user they were incorrect and show which answer was correct
      f) Call the function again OR end
10) When user done, state number instances encountered and % correct overall and by language of origin (call out top/bottom few)

Section C: Word-origin and word-definition memory management
11) Ensure that results/status are written to a CSV/DataFrame
12) Allow user to call functions to summarize/show details of performance on word-origin and word-definition
13) Give user the option of resetting the log file
