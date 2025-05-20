# QueryGPT - AI-Powered Question-Answering System 🤖📚

This project, **QueryGPT**, is a Python-based AI-powered Question-Answering System that utilizes FAISS for similarity search and GPT-2 for generating human-like responses. The system processes an article, indexes its sentences, and retrieves relevant information to answer user questions.

## ✨ Features
- Uses `sentence-transformers` and FAISS to embed and index sentences from an article.
- Finds the most relevant sentences for a given question.
- Generates human-like responses using GPT-2.
- Provides an interactive chatbot-like question-answering experience.

## 🔧 Installation
Ensure you have Python 3.8+ installed, then install the required dependencies:

```bash
pip install sentence-transformers faiss-cpu transformers colorama nltk
```

## 🚀 Usage
### Run the System
Execute the script with the following command:
```bash
jupyter notebook QueryGPT.ipynb
```

### How It Works?
1. The system asks for the file path of an article.
2. The article is processed, and its sentences are indexed.
3. You can ask questions, and the system will retrieve the most relevant sentences.
4. GPT-2 generates a detailed answer based on the retrieved context.
5. The session continues until you type `exit`.

## 🛠 Code Structure
- **`preprocess_article(article)`**: Splits sentences and embeds them.
- **`create_faiss_index(embeddings)`**: Creates a FAISS index for fast similarity search.
- **`load_article_from_file(file_path)`**: Reads an article from a file.
- **`get_answer(question, sentences, index)`**: Finds relevant sentences and generates an answer.
- **`generate_response(prompt)`**: Uses GPT-2 to generate a human-like response.
- **`format_and_print_response(response)`**: Formats and prints the response.
- **`main()`**: Interactive CLI loop for user queries.

## 💡 Example Usage
```bash
🔹 Enter the file path of your article: /content/drive/MyDrive/v_gpt2/data.txt
👨‍💻 Ask a question (or type 'exit' to quit): What is the main idea of the article?
🤖 QueryGPT:
✨ ❓ Question: What is the main idea of the article?
📖 Relevant Context: "It not only helps in maintaining physical
fitness but also plays a crucial role in improving mental
health. It increases blood flow to the brain, which can
enhance focus, memory, and problem-solving skills." 
🤖 Answer: "It is important to note that the study was conducted in a
small population of people with a high level of physical
activity. The main goal of this study is to understand
the role of exercise in the development of mental and
physical health."
👨‍💻 Ask a question (or type 'exit' to quit): What should we do to live a healthy life?
🤖 QueryGPT:
✨ ❓ Question: What should we do to live a healthy life?
📖 Relevant Context: "The Importance of Regular Exercise Exercise
is an essential part of a healthy lifestyle. Regular physical
activity can prevent many chronic diseases, including heart disease, diabetes,
and obesity."
🤖 Answer: "Regular exercise is a good way to reduce stress and improve your health."
👨‍💻 Ask a question (or type 'exit' to quit): exit
🔚 Chat session ended.
```

## 📦 Dependencies
- `sentence-transformers`: For sentence embeddings.
- `faiss-cpu`: For fast similarity search.
- `transformers`: For GPT-2 text generation.
- `colorama`: For colored terminal output.
- `nltk`: For sentence tokenization.

## 📜 License
This project is licensed under the MIT License.



***Altan Ulaş Zöhre***
 
