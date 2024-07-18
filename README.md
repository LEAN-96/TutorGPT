# TutorGPT

In this repository we will explore how to build a no-code, local and open-source Retrieval-Augmented-Generation (RAG) chatflow using [Flowise AI](https://flowiseai.com/). This project was part of the master program study Digital Business Engineering at the Herman-Hollerith-Zentrum (HHZ) in the lecture Applied Machine Learning 

For the purpose of our project we have built an AI Tutor for the lecture of Distributed System. Our tutor answers questions about the lecture slides in an engaging and motivating tone.


![image](https://github.com/user-attachments/assets/813dff1b-4299-47d5-8dc1-e6ddbd324064)


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

## What is Ollama?

Ollama is an open-source project that serves as a powerful and user-friendly platform for running LLMs on your local machine. It supports a variety of models, including Llama3, Mistral, Gemma etc...

## How to setup Ollama?

1. Download [Ollama](https://ollama.com/) for the OS of your choice.
2. Install ollama.exe
3. Open terminal through cmd and pull [models](https://ollama.com/library) of your choice from Ollama. For our project we compared Google´s Small Language Models [gemma:2b](https://ollama.com/library/gemma:2b), [gemma:7b](https://ollama.com/library/gemma:7b) and [gemma2:9b](https://ollama.com/library/gemma2:9b). As an embedding model we used [nomic-embed-text](https://ollama.com/library/nomic-embed-text).

```ollama pull gemma:2b```

```ollama pull gemma:7b```

```ollama pull gemma2:9b```

```ollama pull nomic-embed-text```

#  Importing the chatflow
After setting up Flowise, Ollama and pulling the models successfully you are ready to start with Flowise using local models. 
> [!IMPORTANT]
> Always make sure Ollama is running in the background. Open [http://127.0.0.1:11434/](http://127.0.0.1:11434/) and it should say "Ollama is running". Flowise should be running in a cmd window as well.

1. On [http://localhost:3000/chatflows](http://localhost:3000/chatflows) click "Add New" on the top right corner to create a blank chatflow
2. Download TutorGPT.json from this repository.
3. Now you should see a blank canvas. We are going to import our chatflow by clicking on the settings icon in the top right corner. Press "Load Chatflow" and import "TutorGPT.json".
4. Save the chatflow



