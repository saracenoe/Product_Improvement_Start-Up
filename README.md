# Product_Improvement_Start-Up

The goal of this proyect was to:
- Detect the topics of dissatisfaction and customer dissatisfaction
- Suggest relevant restaurant photos relevant

## Objectives
Implement ML models to answer the questions: 
- Can we distinguish a negative commentary?
- What are the topics of dissatisfaction customer feedback?
- What does a photo of a restaurant?

## Presentation
Slides with the orkflow of the project.

## Method

### We use two datasets provided by Yelp:
- The Academic dataset: data from 150346 restaurants, ~7 million reviews and 200100 photos annotated.
- YELP GraphQL API: data from 200 restaurants, 1 comment and 1 photo per restaurant (200 comments and 200 photos) comments and 200 photos)

### We are faced with two problems:
- A Natural Language Processing (NLP) problem:
  - Defining whether a comment is positive or negative (sentiment analysis)
  - Identify the subjects of a comment set (topic modeling)

- A Computer Vision (CV) problem:
  - Recognising the content of an image and labelling it (image labelling): multi-class classification

In both cases:
- Extract features:
- Text: "Tokens" = group of words reduced to their simplest form
- Images: "visual words" = SIFT features
- Represent the corpus as a Bag of (visual) Words
- Reduce the size of this representation
- Compare the results with pre-trained models
