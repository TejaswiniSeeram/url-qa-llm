# URL Question Answering with LangChain

Ask any question about any webpage — paste a URL, type your question, 
get an answer grounded in that page's content.

## Demo
Here is the app interface:

![App Screenshot](images/screenshot.png)

## How It Works
1. You paste a URL
2. The app scrapes and chunks the page content
3. LangChain retrieves the relevant chunks
4. An LLM generates an answer based only on that content

## Tech Stack
- Python, LangChain, OpenAI API
- Streamlit (UI)
- BeautifulSoup (web scraping)

## Run Locally
git clone https://github.com/your-username/url-qa-llm.git
cd url-qa-llm
pip install -r requirements.txt
Add your OPENAI_API_KEY to a .env file
streamlit run app.py

## What I Learned
[2-3 sentences about what was technically interesting]
```

The demo screenshot or GIF is the single most important thing in the README. Use a free tool called **ScreenToGif** (Windows) or **Kap** (Mac) to record a 20-second demo of your app working. That one GIF will make 10x more recruiters click through than any amount of text.

---

## THE DAILY GITHUB HABIT

This is simple. Every day you sit down to work:

**Start of day:**
```
git pull
```
Gets any changes (matters more when collaborating, but builds the habit)

**End of day, no matter what:**
```
git add .
git commit -m "what I actually did today"
git push
```

Even if all you did was add comments to your code or update the README. Push something every day. The contribution graph is public and recruiters look at it.

---

## WHAT NOT TO DO

Don't push Jupyter notebooks as your main project file. Notebooks are fine for exploration but your final project should run as a Python script or Streamlit app. Notebooks with outputs look messy and don't deploy.

Don't create a new repo every time you experiment. Experiment in branches:
```
git checkout -b experiment-new-chunking