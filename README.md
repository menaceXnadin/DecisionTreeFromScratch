# Decision Tree from Scratch

A simple decision tree built from scratch in Python to help understand how decision trees work!

## What is this?

This project creates a decision tree without using any fancy machine learning libraries. It's like building a flowchart that asks questions about your data to make predictions.

Think of it like a game of 20 questions - the tree asks questions like "Is the person older than 25?" and based on the answer, it goes left or right until it makes a guess about what the answer should be.

## What data does it use?

The project uses a fun dataset about people's preferences:
- **Loves Popcorn**: Yes or No
- **Loves Soda**: Yes or No 
- **Age**: How old they are (7 to 83 years old)
- **Target**: Do they love the movie "Cool As Ice"? (Yes or No)

The goal is to predict if someone will love the movie based on their other preferences!

## How does it work?

### 1. Finding Good Questions
The tree looks at all possible questions it could ask (like "Are you older than 30?" or "Do you love popcorn?") and picks the best one that separates people into groups.

### 2. Splitting Data
Once it picks a question, it splits people into two groups - those who answer "yes" and those who answer "no".

### 3. Measuring How Good a Split Is
It uses something called "Gini impurity" (fancy name for "how mixed up are the groups?"). Pure groups (all yes or all no) are good, mixed groups are bad.

### 4. Building the Tree
It keeps asking questions and splitting groups until everyone in a group gives the same answer, or it reaches a maximum number of questions.

### 5. Making Predictions
When you want to predict something new, you follow the questions from top to bottom until you reach an answer.

## What's cool about this?

- **No cheating**: Built from scratch without using existing machine learning libraries
- **Handles different data**: Works with both yes/no questions and numbers
- **Won't overfit**: You can limit how many questions it asks to keep it simple
- **Easy to understand**: You can see exactly what questions it's asking

## How to use it

1. **Get your data ready**: Put your data in a table (pandas DataFrame)
2. **Build the tree**: Tell it which column has the answers you want to predict
3. **Make predictions**: Give it new data and it will make a guess!

## What you need

- Python 3.x
- pandas (for handling data tables)
- numpy (for math stuff)
- collections (already included with Python)

## Why is this useful for learning?

This project helps you understand:
- How computers make decisions step by step
- Why some questions are better than others for splitting data
- How to build something complex by breaking it into simple parts
- The basics of machine learning without getting lost in complicated libraries

## What could make it even better?

- Add different ways to measure how good a split is
- Make it smarter about when to stop asking questions
- Handle missing data (when someone doesn't answer a question)
- Add pretty pictures to visualize the tree

## Final note

This is made for learning! It shows you how decision trees work under the hood, which is super helpful before you start using the fancy pre-built ones.
