# 📚 GPTWiki

**GPTWiki** automatically turns random internet content into clean, structured Wikipedia-style articles — and uploads them to your MediaWiki site.

It uses OpenAI-compatible LLMs to:
- 🎯 Extract real academic-style topics from raw text (e.g., Random Reddit posts)
- 📝 Write full articles in MediaWiki format (6+ sections, encyclopedic tone)
- 🌐 Upload everything to your wiki via API — 24/7, no human needed

You control the prompts and source. GPTWiki handles the writing, structuring, and publishing.


---

## 🚀 Key Features

- 🔍 **Ingest any data** — Reddit, Stack Overflow, RSS, crawled posts, etc.
- 🧠 **Auto-generate specific academic titles** via LLM prompt
- 📄 **Write full encyclopedic articles** in MediaWiki markup
- 📂 **Auto-generate categories**
- 🌐 **Directly uploads to MediaWiki** via API
- 🔁 **Overwrite mode** or skip existing pages
- 🧵 **Multithreaded background loop**
- 🧩 100% customizable: Bring your own data, prompt, and endpoint

---

## ⚙️ How It Works

1. **Collect Data**  
   Use any text source. The built-in example uses Reddit API to fetch recent CS-related discussions.

2. **Generate Title**  
   LLM turns the noisy input (e.g., a Reddit post) into a real academic-style topic

3. **Generate Article**  
   With your prompt template, GPTWiki creates a long MediaWiki-formatted article with 6+ sections.

4. **Auto Categorize**  
   GPT generates relevant categories (e.g., *Artificial Intelligence*, *Cognitive Science*) for indexing.

5. **Upload**  
   Articles are uploaded to your MediaWiki instance via API. You can choose to:
   - 🚫 Skip if the page exists
   - 🔄 Force overwrite for updates

---

## 🌍 Data Source: Anything Text

Although our example uses Reddit API, you can plug in:

- 🔥 Reddit / Stack Overflow
- 📖 Academic abstracts
- 🌐 RSS feeds, blogs
- 🧠 Internal datasets
- 🛠️ Even a simple .txt file

> Just make sure each line is a string-like topic or article seed.

---

## 💻 See It Running

🔗 [EdwardWiki](https://wiki.t.us.kg) — 100% generated with GPTWiki  
Fetches Reddit posts, converts to advanced research topics, writes full-length Wikipedia-style articles, and auto-publishes to MediaWiki.

---

## 📂 Usage

See [`example.py`](./example.py) — full working script that:

- Uses Reddit API for topic input
- Generates titles via prompt
- Produces long-form MediaWiki content
- Classifies and uploads to your MediaWiki
- Runs in multithreaded infinite loop

---

## 🧬 Inspiration

**GPTWiki** is inspired by [LSJBOT](https://en.wikipedia.org/wiki/LSJBOT), the bot that created millions of Wikipedia articles using static datasets.

Unlike LSJBOT, GPTWiki demonstrates that **modern LLMs + live APIs** (e.g. Reddit) can generate structured, high-quality encyclopedia articles — **with zero human editing**.

> It proves that full-scale, autonomous wiki generation is now viable using public data and AI.

