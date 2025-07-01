# 🌍 Multilingual Company Brochure Generator

This project allows you to **automatically generate a company brochure** by simply entering a website URL, selecting a tone (e.g., professional, jovial), and choosing a language. The app uses OpenAI's `gpt-4o-mini`, `BeautifulSoup` for web scraping, and `Gradio` for a no-code UI experience — all running inside Google Colab.


## ✨ Features

- 🔍 Scrape content from any public company website
- 🧠 Use GPT-4o-mini to filter relevant links (About, Careers, etc.)
- 📝 Generate a brochure in your chosen tone (e.g., professional, luxury)
- 🌐 Translate brochure into 15+ languages
- ⚡ Easy-to-use Gradio interface
- 🔒 Secure API key handling using Colab Secrets


## 📦 Dependencies

Install all required Python packages using:

```bash
!pip install -q openai python-dotenv beautifulsoup4 gradio
````


## 🔐 Setup in Google Colab

1. Open the notebook in Google Colab.
2. Run the following once to set your OpenAI API key securely:

```python
from google.colab import userdata
userdata.set_secret("OPENAI_API_KEY")
```


## 🛠️ How It Works

### Step-by-Step:

1. **Scrape Website**
   Extract clean text and all hyperlinks using `BeautifulSoup`.

2. **Filter Relevant Links with GPT**
   Ask GPT-4o-mini to pick the links that are brochure-worthy (e.g., /about, /careers).

3. **Fetch Content from Subpages**
   Load and clean all selected subpages.

4. **Generate a Brochure**
   Prompt GPT to generate a short, markdown-formatted company brochure.

5. **Translate (Optional)**
   If language ≠ English, GPT is prompted to translate the output.

6. **Render in Gradio UI**
   Users interactively input the company name, tone, and language to generate brochures.



## 🎨 Gradio UI Preview

* **Inputs**: Company name, website URL, tone, and language
* **Output**: Markdown-rendered brochure
* **Languages Supported**: English, Hindi, Mandarin, French, Spanish, German, Japanese, and more
* **Tones Supported**: Professional, Jovial, Luxury, Youthful, Serious, Friendly, Inspirational



## 🌐 Example Use Cases

| Company   | Tone         | Language         |
| --------- | ------------ | ---------------- |
| CNN       | Professional | American English |
| Apple     | Luxury       | French           |
| Bytedance | Jovial       | Hindi            |
| WHO       | Serious      | Spanish          |



## 🚀 Run the App

```python
demo.launch()
```

Once launched, Gradio will provide a public shareable URL in Colab.



## 💡 Extension Ideas

* [ ] Export brochure to PDF or DOCX
* [ ] Support batch processing of URLs
* [ ] Add company logo scraping
* [ ] Integrate with Notion, Webflow, or CMS
* [ ] Auto-detect tone and preferred language from region



## 📄 License

MIT License



## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change or improve.



## 🙌 Acknowledgements

* [OpenAI GPT-4o-mini](https://platform.openai.com/docs)
* [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/)
* [Gradio](https://gradio.app/)
* [Google Colab](https://colab.research.google.com/)



