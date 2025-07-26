# 📚 Book Recommendation System

This project is an AI-powered book recommendation system that uses vector embeddings and large language models to suggest books based on user interests. It leverages Gradio for the front-end interface and supports both Google Generative AI and Hugging Face embeddings via LangChain.

---

## 🚀 Features

- 🔍 Semantic search from book descriptions
- 📖 Input user interest and receive relevant book suggestions
- 🧠 Vector embeddings powered by Google Gemini or Hugging Face
- 🌐 Deployable on Render with minimal configuration
- 🎛️ Gradio dashboard for an interactive UI

---

## 🛠️ Tech Stack

- Python 3.10+ (tested on 3.12/3.13)
- LangChain
- Gradio
- ChromaDB (Vector DB)
- Google Generative AI (models/embedding-001) or Hugging Face Transformers
- Render (for deployment)

---

## 📁 Dataset

7K books - https://www.kaggle.com/datasets/dylanjcastillo/7k-books-with-metadata
**Example Format:**

```
Book Title: The Alchemist
Description: A philosophical story about a shepherd's journey of finding meaning and purpose.
---
Book Title: Atomic Habits
Description: A practical guide on building good habits and breaking bad ones.
```

---

## ⚙️ Installation & Local Setup

```bash
git clone (https://github.com/pratp-123/book-recommendation-llm/new/main?filename=README.md)
cd book-recommendation-llm

# Create a virtual environment
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

# Install dependencies from cmd
pip install -r requirements.txt

# Run the app
python gradio-dashboard.py
```

Make sure to place `tagged_description.txt` in the root directory.

---

## 🌍 Deployment (Render)

1. Push this project to a GitHub repo.
2. Connect it with [Render](https://render.com).
3. Set build command:
   ```
   pip install -r requirements.txt
   ```
4. Set start command:
   ```
   python gradio-dashboard.py
   ```
5. Set Environment Variables if using Google API:
   ```
   GOOGLE_API_KEY = <your_api_key>
   ```

---

## 🔐 Authentication Note (Google Generative AI)

To use Google Generative AI embeddings, ensure you’ve set up:
- Application Default Credentials (ADC)
- Enabled `generativelanguage.googleapis.com` in your Google Cloud Console

🔗 [How to set up credentials](https://cloud.google.com/docs/authentication/external/set-up-adc)

---

## 📜 License

This project is licensed under the MIT License.

---

## 🤝 Contribution

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

---

## 🙋‍♂️ Author

**Prateek Chauhan**  
[GitHub](https://github.com/pratp-123) | [LinkedIn](https://www.linkedin.com/in/prateek-chauhan-291301218/)
