![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9A825.svg?style=for-the-badge&logo=googlecolab&logoColor=white)![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)

## LLM LlamaIndex
В коде реализован подход с фиксированием версий ряда библиотек с которым работает готовый продукт. Это сделано для удобства и стабильности кода.

> Также для использования кода рекомендуется использовать
> сгенерированный токен на **[HuggingFace](https://huggingface.co/settings/profile)** в настройках вашего профиля.

Здесь используется модель *[IlyaGusev/saiga_mistral_7b](https://huggingface.co/IlyaGusev/saiga_mistral_7b_gguf)*. 
В качестве эмбеддинга будем использовать *[sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2](https://huggingface.co/sentence-transformers/paraphrase-multilingual-MiniLM-L12-v2)*, которая хорошо работает с разными языками. 
В качестве базы знаний, которая подается в *RAG-систему* будет использовать данная [статья](https://ru.wikipedia.org/wiki/TensorFlow). 

Также в коде представлена простая реализация **Gradio-интерфейса** с базовым функционалом: *распарсить данные* и *отправить запрос*. 

Важно!

> Этот код получится выполнить только с использованием аппаратного
> ускорителя. Я использовал графический **ускоритель T4** в **Google Colab**.
