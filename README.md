
# Book Recommendation Chatbot using IBM Watson Assistant

## Overview

This project is developed as part of the **IBM PBEL Virtual Internship**.  
The chatbot provides book recommendations based on the user’s genre preferences, mood, favorite authors, and reading level. It uses IBM Watson Assistant to simulate natural conversations and deliver personalized book suggestions.

## Objectives

- Build a conversational chatbot using IBM Watson Assistant
- Understand user input using NLP to recommend relevant books
- Capture key details such as genre, mood, or author using slots and entities
- Provide fallback responses and guide users who are unsure

## Tools & Technologies

- IBM Watson Assistant – For intent detection, entity recognition, and dialog flow
- IBM Cloud – Platform hosting the assistant
- CSV Files – Used to upload entity values in bulk
- JSON Files – Used for skill export and import
- GitHub – For version control and final submission

## IBM Watson Concepts Used

- **Intents**: Represent what the user is trying to do  
  Example: Asking for a book, greeting the bot, or saying goodbye.

- **Entities**: Keywords that provide specific details  
  Example: Genre (fantasy), Mood (happy), Author (Dan Brown)

- **Dialog Nodes**: Predefined paths based on intents/entities that decide how the bot should respond

- **Slots**: Automatically gather missing pieces of information (like asking for genre if not mentioned)

## Intents

| Intent Name        | Purpose                                      |
|--------------------|----------------------------------------------|
| `#Greeting`        | Recognize and reply to greetings             |
| `#Goodbye`         | Exit conversation politely                   |
| `#Genre_Search`    | Book request based on genre                  |
| `#Mood_Based`      | Book suggestions based on mood               |
| `#Author_Search`   | Books by specific author                     |
| `#ReadingLevel`    | Recommendations for teens, beginners, etc.   |
| `#Need_Help`       | User doesn't know what they want             |
| `#Fallback`        | Default response for unrecognized input      |

## Entities

| Entity Name        | Example Values                                  |
|--------------------|-------------------------------------------------|
| `@genre_entity`    | fantasy, romance, thriller, sci-fi, horror      |
| `@mood_entity`     | happy, sad, stressed, bored                     |
| `@author_entity`   | J.K. Rowling, Agatha Christie, Dan Brown        |
| `@readinglevel`    | beginner, teen, adult, expert                   |

## Inputs and Expected Outputs

| User Input                                 | Bot Response                                                |
|--------------------------------------------|-------------------------------------------------------------|
| "Suggest a fantasy book"                   | "Try *Mistborn* by Brandon Sanderson."                      |
| "I'm feeling anxious"                      | "You might like *The Midnight Library* by Matt Haig."       |
| "Books by Dan Brown"                       | "*Inferno* and *The Da Vinci Code* are great picks."        |
| "I'm a teen, what should I read?"          | "*Percy Jackson* is a great read for teenagers."            |

## Files Included

- `skill_export.json` – Main chatbot logic from IBM Watson Assistant
- `genre_entity.csv`, `mood_entity.csv` – Entity value uploads
- `BookBot_Explanation.ipynb` – Jupyter notebook explaining the flow and logic

## Future Enhancements

- Add book review APIs (like Goodreads or Google Books)
- Filter by publication year, language, or popularity
- Deploy chatbot on a website or mobile app interface

## Made By

[GitHub Profile – Riddhi](https://github.com/riddhi1909)
