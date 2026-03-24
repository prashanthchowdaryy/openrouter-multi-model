# OmniAI-Chat

A simple multi-model AI chatbot built using OpenRouter.

I made this to experiment with different LLMs (Gemini, Grok, DeepSeek, Kimi) in one place, instead of switching between tools. The goal was to understand how these models behave, how reasoning works, and how to manage things like tokens, errors, and responses properly.

---

## What this project does

* Connects to multiple AI models through OpenRouter
* Supports follow-up questions (basic conversation flow)
* Handles reasoning-based models like Kimi
* Cleans up API responses (no messy JSON output)
* Includes basic error handling
* Controls token usage to avoid credit issues

---

## Models used

* Gemini (fast + lightweight reasoning)
* Grok (xAI)
* DeepSeek
* Kimi (thinking / reasoning model)

All of these are accessed through OpenRouter.

---

## Why I built this

At first, I was just calling APIs and printing responses.
But things got messy quickly — errors, token limits, weird outputs.

So I decided to build something cleaner:

* structured requests
* proper response handling
* reusable logic

This project is basically my way of learning how real AI systems are put together.

---

## Setup

Clone the repo:

```bash
git clone https://github.com/your-username/OmniAI-Chat.git
cd OmniAI-Chat
```

Install requirements:

```bash
pip install requests
```

---

## API Key

Get your API key from OpenRouter and add it in the code:

```python
API_KEY = "your_openrouter_api_key"
```

Don’t push your key to GitHub.

---

## Run

```bash
python main.py
```

---

## Example

Input:

```
How many r's are in strawberry?
```

Output:

```
3
```

---

## What I learned

* How to work with LLM APIs properly
* Why error handling matters (a lot)
* How token limits affect cost
* How to structure responses instead of dumping raw JSON
* Difference between basic models and reasoning models

---

## Future improvements

* Simple UI (maybe Streamlit)
* Chat history / memory
* Model selection option
* Better project structure

