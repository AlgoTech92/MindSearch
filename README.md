<div id="top"></div>

<div align="center">

<img src="assets/logo.svg" style="width: 50%; height: auto;">

[🌐 Project Page](https://mindsearch.netlify.app/) | [📃 Paper](<>) | [💻 Playground](https://mindsearch.openxlab.org.cn/)

English | [简体中文](README_zh-CN.md)

https://github.com/user-attachments/assets/0e5bdfa1-dad9-4f17-968d-2b812e64bf15

</div>
</p>

## ✨ MindSearch: Mimicking Human Minds Elicits Deep AI Searcher

MindSearch is an open-source AI Search Engine Framework with Perplexity.ai Pro performance. You can simply deploy it with your own perplexity.ai style search engine with either close-source LLMs (GPT, Claude) or open-source LLMs (InternLM2.5-7b-chat). It owns following features:

- 🤔 **Ask everything you want to know**: MindSearch is designed to solve any question in your life and use web knowledge.
- 📚 **In-depth Knowledge Discovery**: MindSearch browses hundreds of web pages to answer your question, providing deeper and wider knowledge base answer.
- 🔍 **Detailed Solution Path**: MindSearch exposes all details, allowing users to check everything they want. This greatly improves the credibility of its final response as well as usability.
- 💻 **Optimized UI Experimence**: Providing all kinds of interfaces for users, including React, Gradio, Streamlit and Terminal. Choose any type based on your need.
- 🧠 **Dynamic Graph Construction Process**: MindSearch decomposes the user query into atomic sub-questions as nodes in the graph and progressively extends the graph based on the search result from WebSearcher.

<div align="center">

<img src="assets/teaser.gif">

</div>

## ⚡️ MindSearch vs other AI Search Engines

Comparison on human preference based on depth, breadth, factuality of the response generated by ChatGPT-Web, Perplexity.ai (Pro), and MindSearch. Results are obtained on 100 human-crafted real-world questions and evaluated by 5 human experts\*.

<div align="center">
<img src="assets/mindsearch_openset.png" width="90%">
</div>
* All experiments are done before July.7 2024.

## ⚽️ Build Your Own MindSearch

### Dependencies Installation

```bash
pip install -r requirements.txt
```

### Setup MindSearch API

Setup FastAPI Server.

```bash
python mindsearch/app.py
```

### Setup MindSearch Frontend

Providing following frontend interfaces:

- React

```bash
cd frontend/React
npm install
npm start
```

- Gradio

```bash
python frontend/gradio.py
```

- Streamlit

```bash
streamlit run frontend/streamlit.py
```

## 🐞 Debug in Locally

```bash
python mindsearch/terminal.py
```

## License

This project is released under the [Apache 2.0 license](LICENSE).