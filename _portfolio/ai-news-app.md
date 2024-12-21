---
layout: project-item
title: "3News App Using Angular, LangChain and OpenAI"
backendRepository: https://github.com/TheAttentionSeeker5050/3-news-backend-fastAPI-LangChain-LLM
frontendRepository: https://github.com/TheAttentionSeeker5050/3-news-frontend-Angular
---

<p id="heading-p">
    3News is an is an app that returns the latest news articles based on the type of news requested, powered by large language models (LLMs) and LangChain. The Python API serves as an interface between the browser client and supports five different news categories: local, international, business, tech, and sports. It processes requests dynamically based on the type of news and location (if needed). The frontend serves as a user interface to access the latest news articles across five categories: local, international, business, tech, and sports.
</p>

## Features
- Five types of news: Local, International, Business, Tech, and Sports.
- Location support: Location can be provided for specific news categories like local and business.
- LLM-powered: Leverages LangChain and OpenAI's GPT-4 for generating and selecting relevant news based on the input.

### News Types Supported
- Local: News based on a provided location (e.g., city, country).
- International: News on global events.
- Business: Business-related news tailored to a specific region or globally.
- Tech: News related to technology trends.
- Sports: Sports-related news, optionally filtered by location.

**Note:** The input is not case-sensitive, but it is spelling-sensitive. Make sure to use the exact names for the news types (e.g., local, not Local).

## Disclaimer
At the current moment, the application is not displaying the latest news because it uses the `gpt-4-turbo` model, which does not have access to live news data. Instead, the news data available is up to April 2023. However, newer versions of the model with live data capabilities can be integrated in the future to provide up-to-date news.