

```R
---
title: Computational text analysis
author: Arindam Basu
---
```


```R
## How to work with these lessons
- Visit [Jupyter Notebook for the project](https://arinsclasses.info.tm:8000/teaching/user/<your_username>/lab)
- Log in with your username and password
- Follow the instructions as I post them on screen and work
- If you get stuck, stick the red sticky note on your computer
- If you can accomplish the task, leave a green sticky note on your computer lid
---
## Session 1: Log in and warm up
- 9:00-9:30: Introduction and warm up 
- select(), filter(), arrange(), summarise() group_by(), mutate()
- gather(), and spread()
- 9:30-9:40: 10-minute break
- 9:40-10:00: Hands on ggplot() graphing
---
## Session 2: read text, corpus, tokens
- Creating corpus using quanteda
- Tokenising documents with tidytext and quanteda
- Using document feature matrix (dfm()) with quanteda
- 10:30-10:40 am - break and stretch yourself
- Word frequencies, term frequencies
- Concepts of Wordcloud, graphing, tf_idf
---
## Session 3: Sentiment analysis
- 10:40 - 11:00 am
- Using dicionaries in quanteda
- Using AFINN, Bing, NRC in tidytext
- Graphing
---
## Session 4: Topic modelling, document classification
- Topic modelling with latent dirichlet allocation
- Topic modelling using quanteda
- Topic modelling with tidytext
- Interpretation of beta
- Document classification
---
## Session 5: Wrap up
- Key lessons
- Feedback forms, fill in link
- [Link for the form](https://docs.google.com/forms/d/e/1FAIpQLSePNSahg6WS_652Dpg8K0TFNoVj-mNkU5w5Kc9fHw1Ms7UMiA/viewform?usp=pp_url&entry.165664929=I+liked+that+...&entry.1261510625=I+did+not+like+or+got+confused+about+...&entry.1466204505=me@somemail.com)
---

## Features of tidy data and R
- tidy data has the following three properties
- Every observation or unit of observation has its own row
- Every feature of observation has its own column
- Every cell has only one information
- You can use tidy principles in conducting text data analysis
---
## Operations in tidyverse
- `%>%` stands for pipe
- This symbol is literally interpreted as 'then'
- `x %>% y` means x THEN y
- The above code says 
> load `mtcars` THEN show header data
---
## In text data analysis
- tidytext, each word or sentence will have its own row
- Each word in a corpus will have its features listed in columns
- We will summarise and operate on the word level data
- Alternatively, you can have sentence level data or 
- You can have character level data to work with
---
## Grammar of tidy data, part I
- `select()` selects columns
- `filter()` filters the rows based on conditions on columns
- `arrange()` rank orders variables in specified order
- `mutate()` create new variables from existing columns
- `group by() %>% summarise()` can summarise groups of data
---
## More with tidy data
```
