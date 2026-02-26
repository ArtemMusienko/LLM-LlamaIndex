![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9A825.svg?style=for-the-badge&logo=googlecolab&logoColor=white)![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)![HuggingFace](https://img.shields.io/badge/huggingface-%23FFD21E.svg?style=for-the-badge&logo=huggingface&logoColor=white)

## LLM LlamaIndex

[![ru](https://img.shields.io/badge/README_на_русском-2A2C39?style=for-the-badge&logo=github&logoColor=white)](README.ru.md)  

The code implements an approach with fixing versions of a number of libraries, with which the finished product works. This is done for the convenience and stability of the code.

> To use the code, use
> the generated token on **[HuggingFace](https://huggingface.co/settings/profile)** in your profile settings.

For a general understanding, let's analyze the important terms in this work:

---

**Llama Index** is a framework for creating applications that work with their own data, based on large language models. It provides tools for indexing, processing, and integrating diverse data sources into a structured format that is understandable to **LLM**. Its primary objective is to effectively extract relevant information and contextualize it to improve the model's responses. As a result, **Llama Index** serves as a powerful bridge between private data and the capabilities of language models.

**Gradio** is an open-source library for quickly creating user-friendly web interfaces for machine learning and other Python programs. It allows you to develop interactive model demos with just a few lines of code, offering ready-made components like input fields, sliders, and graphs. With its ease of use, **Gradio** accelerates the process of testing, sharing, and deploying models. This makes machine learning models more accessible to users without a technical background.

---

This example uses the *[IlyaGusev/saiga_mistral_7b](https://huggingface.co/IlyaGusev/saiga_mistral_7b_gguf)* model. As embedding, we will use *[sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2)*, which works well with different languages.

 As the knowledge base that is fed into the *RAG system*, we will use this [article](https://ru.wikipedia.org/wiki/TensorFlow).

The code also provides a simple implementation of the **Gradio interface** with basic functionality: *parse data* and *send a request*.

Important!

> This code can only be executed using a hardware
> accelerator. I used a **T4 graphics accelerator** in **Google Colab**.