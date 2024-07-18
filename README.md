# TutorGPT

In this repository we will explore how to build a no-code, local and open-source Retrieval-Augmented-Generation (RAG) chatflow using [Flowise AI](https://flowiseai.com/). This project was part of the master program study Digital Business Engineering at the Herman-Hollerith-Zentrum (HHZ) in the lecture Applied Machine Learning 

For the purpose of our project we have built an AI Tutor for the lecture of Distributed System. Our tutor answers questions about the lectures slides in an engaging and motivating tone.

# Pre-Requirements 
Before you can import the chatflow you need to have Flowise and Ollama installed. 

## What is Flowise?

Flowise is an open source low-code tool for developers to build customized LLM orchestration flows & AI agents. Through a simple drag-and-drop UI approach it allows you to quickly prototype LLM applications.

## How to install Flowise?
Since we wanted to use all components of our system locally, we deployed Flowise locally using NPM. For other deployment options head over to their [documentation](https://docs.flowiseai.com/getting-started) or [Github](https://github.com/FlowiseAI/Flowise).

1. Install [NodeJS](https://nodejs.org/en/download/package-manager) (Node v18.15.0 or v20)
2. Open terminal through cmd and install Flowise
```npm install -g flowise```
3. After installing start Flowise in the terminal
```npx flowise start```
4. Open: [http://localhost:3000](http://localhost:3000)
> [!TIP]
> Download flowise_temp.bat file. Executing this file with automatically start and open Flowise.
5. Update Flowise:
```npm update -g flowise```



