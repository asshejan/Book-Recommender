# 📚 Semantic Book Recommender

![Semantic Book Recommender Preview](preview.png)

Discover books that fit your mood, category, or desired tone with **Semantic Book Recommender**. This project combines the power of AI embeddings from Hugging Face, natural language processing, and a user-friendly Gradio interface to deliver a personalized book recommendation experience.

---

## 🚀 Features

- **Natural Language Search**: Find book recommendations based on a description or a query in natural language.
- **Category Filtering**: Refine your results by selecting specific book categories (e.g., Fiction, Self-help).
- **Emotional Filtering**: Get book recommendations based on emotional tones like Happy, Sad, Suspenseful, and more.
- **User-friendly Interface**: Built using Gradio, making it interactive and accessible for all users.

---

## 🛠️ How It Works

The **Semantic Book Recommender** uses the following steps:
1. Loads a dataset of books with metadata, emotional scores, and descriptions.
2. Leverages Hugging Face's `sentence-transformers/all-MiniLM-L6-v2` model to generate embeddings for book descriptions.
3. Embeds user queries using the same model.
4. Retrieves the most semantically similar books using **Chroma** as the vector database engine.
5. Filters recommendations further based on user-selected category and emotional tone.

---

## 🖼️ Preview

![Book Recommender App Preview](preview.png)

---

## 📑 Project Structure

```bash
.
├── app.py                  # Main application file with Gradio logic
├── books_with_emotions.csv # Dataset containing books metadata, emotions, and thumbnails
├── tagged_description.txt  # File with tagged descriptions for semantic embeddings
├── requirements.txt        # List of Python dependencies
├── .env                    # Environment variables (for any OpenAI & Huggingface API keys)
└── README.md               # This README file
```

---

## ⚙️ Installation and Usage

To run the **Semantic Book Recommender** locally:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/asshejan/Book-Recommender.git
   cd Book-Recommender
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Application**:
   ```bash
   python app.py
   ```

4. Open your browser and go to `http://127.0.0.1:7860`.

---

## 🛠️ Dependencies

Make sure you have the following libraries installed (or listed in `requirements.txt`):
- `gradio`
- `langchain`
- `sentence-transformers`
- `pandas`
- `numpy`
- `python-dotenv`
- `chromadb`

You can install them with:
```bash
pip install -r requirements.txt
```

---


## 🙌 Contribute

Feel free to contribute to the **Semantic Book Recommender** by:
- Submitting bug reports or feature requests.
- Adding new functionality (e.g., more emotional tones, better search algorithms).
- Cleaning and improving the existing code.

---

## 📧 Support

If you have any questions or run into issues, feel free to contact me:
- GitHub: [Your GitHub Profile](https://github.com/asshejan)

---

## 🌟 Acknowledgements

Special thanks to:
- **Hugging Face** for their awesome `sentence-transformers`.
- **Gradio** for making interactive machine learning applications easy to build.
- **LangChain** for simplifying AI workflows.

---

Enjoy discovering a world of books with **Semantic Book Recommender**! 📚✨
