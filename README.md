# QUERIES ABOUT PDF FILES USING LLM WITH RAG
## Description
This project demonstrates a simple application of Retrieval-Augmented Generation (RAG) for enhancing the question-and-answer experience with lesson materials related to AIO 2024. RAG is an AI technique that combines the strengths of retrieval-based and generative models to provide more accurate, relevant, and contextually aware responses.

This project includes:

- Building a simple RAG program by [Langchain](https://python.langchain.com/v0.2/docs/introduction/)
- Using the [Vicuna](https://lmsys.org/blog/2023-03-30-vicuna/) model, an open-source large language model that can respond well to Vietnamese
- Building a chat interface to get a complete chat app with [Chainlit](https://docs.chainlit.io/get-started/overview)


## Installation

#### Running the Notebook on your computer

1. *Clone the repository:*
    ```sh
    git clone https://github.com/tranphuongtruc/QUERIES_ABOUT_PDF_FILES_USING_LLM_WITH_RAG.git
    cd QUERIES_ABOUT_PDF_FILES_USING_LLM_WITH_RAG
    ```

2. *(Optional)Create a virtual environment:*
   
    On Windows:
 
    ```sh
    python -m venv venv
    .\venv\Scripts\activate
    ```

    On macOS and Linux:

    ```sh
    python3 -m venv venv
    source venv/bin/activate
    ```

#### Running the Notebook on Google Colab

1. *Open Google Colab*

    Go to [Google Colab](https://colab.google/)

2. Upload Your Notebook

    Click on ***File*** -> ***Upload notebook***
    Choose the .ipynb file from your local machine.

3. *(optional) Mount Google Drive*

    If your notebook requires access to files stored in your Google Drive, you can mount it using the following code:

    ```sh
    from google.colab import drive
    drive.mount('/content/drive')
    ```


#### NOTES

When reading a PDF file, make sure to check the FILE_PATH carefully

```sh
Loader = PyPDFLoader
FILE_PATH = "/content/YOLOv10_Tutorials.pdf"
loader = Loader(FILE_PATH)
documents = loader.load()
```
