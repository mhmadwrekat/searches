## RASA

Rasa provides the standard infrastructure layer for conversational AI.

---

<!-- **How to get user preferences from cookies ?** -->

## What is Rasa AI?

Rasa is a _framework_ for developing AI powered, industrial grade chatbots. It’s incredibly powerful, and is used by developers worldwide to create chatbots and contextual assistants.

Rasa is an open source machine learning framework for building AI assistants and chatbots. Mostly you don’t need any programming language experience to work in Rasa. Although there is something called “Rasa Action Server” where you need to write code in Python, that mainly used to trigger External actions like Calling Google API or REST API.

---

## Rasa has two main modules!

**1. Rasa NLU for understanding user messages.**

- Rasa NLU — This is the place, where rasa tries to understand User messages to detect Intent and Entity in your message. Rasa NLU has different components for recognizing intents and entities, most of which have some additional dependencies.

**2. Rasa Core for holding conversations and deciding what to do next.**

- Rasa Core — This is the place, where Rasa try to help you with contextual message flow. Based on User message, it can predict dialogue as a reply and can trigger Rasa Action Server.

**Now Rasa NLU and Rasa Core source code are merged together.**

---

###### Architecture of RASA

![Architecture of RASA](https://editor.analyticsvidhya.com/uploads/77211a.png)

---

### Install Rasa

- use miniconda to avoid the issue with other installed Python packages in your system or conflicting Python Version.
- use the commands :

```
conda install python=3.6
conda create -n rasa python=3.6
source activate rasa
pip install rasa-x --extra-index-url https://pypi.rasa.com/simple
```

---

### some simple concepts that we should know while creating a chatbot.

**_Query_**
A query is the user message for the chatbot in order to get details of something.

**_Response/Action_**
Action is the response from a chatbot based on the query.

**_Intents_**
Intents can be described as the aim or intention of the user input.

_For example, hii, hello, good morning, good evening, etc.. can be treated as greeting intent._

**_Entities_**
Entities can be described as useful information that can be extracted from the user input ( The nouns in the dialogue).

_For example, “‘I want to book a ticket from DELHI to COCHIN”, here both Delhi and Cochin are entities(location)_

---

## Rasa Configuration

files which are created as Initial project structure of Rasa:

- `__init__.py` an empty file that helps python find your actions.

- `actions.py` code for your custom actions. In-case you want Rasa to call external server via REST API or API call, you can define your Custom Actions here. Remember you can create multiple Python Script for Rasa Custom Action.

- `config.yml` configuration of your NLU and Core models. In-case you are dealing with Tensorflow or Spacy, you need to define such pipeline here. To handle this file, you show know about Machine Learning and Deep Learning.

- `credentials.yml` details for connecting to other services. In case you want to build Bot on Facebook Messenger, Microsoft Bot Framework, you can maintain such credential and token here. So basically you just need to add Facebook, slack and Bot framework related configuration, rasa will automatically do rest for you. Remember that you need to host Rasa over https domain. During development, you can use ngrok as a testing tool.

- `data/nlu.md` your NLU training data. Here you can define Intent. Like Order Pizza or Book Uber. You need to add related Sentences for that Intent. Remember if you are using Rasa-X, your training Intent and Data will be added automatically.

- `data/stories.md` your stories. This is required for Rasa Core. There is something called “Dialog Flow in Rasa” where Rasa Core controls the flow of the conversation between you and chatbot, so for that flow, you need to train chatbot using these stories. So in case you want your chatbot to be very perfect on different context (stories) you can add those stories here.

- `domain.yml` your assistant’s domain. This file combines Different Intent which chatbot can detect and list of Bot replies. Remember you can define your Custom Action Server Python method name here (in underscore format), so that Rasa will call that python method for you.

- `endpoints.yml` details for connecting to channels like FB messenger. This is mainly used for production setup. You can configure your Database like Redis so that Rasa can store tracking information.

- `models/<timestamp>.tar.gz` your initial model.

![RASA](https://i.ytimg.com/vi/sazsWmP2d3o/maxresdefault.jpg)

---

### Reference

1. [Article 1](https://towardsdatascience.com/create-chatbot-using-rasa-part-1-67f68e89ddad)

2. [Article 2](https://www.analyticsvidhya.com/blog/2021/11/an-introduction-to-chatbot-development-using-rasa/)

3. [Youtube Video](https://www.youtube.com/watch?v=Ap62n_YAVZ8&t=181s)

4. [RASA Website](https://rasa.com/)

---
