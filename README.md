# 🔎 Keyword & Topic Extractor

A simple web-based **Keyword & Topic Extraction** application that analyzes text, identifies important words, calculates their frequency, and detects possible topics using a rule-based Natural Language Processing approach.

The application presents extracted keywords through rankings, frequency bars, a keyword cloud, and topic tags.

---

## 📌 Project Overview

The **Keyword & Topic Extractor** helps users quickly understand the main concepts contained in a piece of text.

The application processes the entered text, removes common stop words, calculates word frequencies, identifies important keywords, and compares the text against predefined topic categories.

It runs completely in the browser without requiring an external API or backend server.

---

## 🎯 Objectives

* Extract important keywords from text.
* Calculate keyword frequency.
* Remove common stop words.
* Identify possible topics.
* Display keywords in ranked order.
* Generate a visual keyword cloud.
* Provide basic text statistics.
* Store recent analyses using LocalStorage.

---

## ✨ Features

* 🔑 Keyword extraction
* 📊 Keyword frequency analysis
* 🏆 Top 10 keyword ranking
* 📈 Keyword frequency bars
* ☁️ Keyword cloud
* 🏷️ Topic detection
* 📝 Total word count
* 🔤 Unique word count
* 🕘 Recent analysis history
* 💾 LocalStorage support
* 🧹 Clear/reset option
* 📱 Responsive design
* ⚡ Runs completely in the browser

---

## 🛠️ Technologies Used

* **HTML5** — Structure
* **CSS3** — Interface and responsive design
* **JavaScript** — Text processing and analysis
* **LocalStorage** — Analysis history
* **Regular Expressions** — Word extraction
* **NLP Concepts** — Stop-word removal, frequency analysis, keyword extraction

---

## 🧠 How It Works

The application follows this process:

```text
User enters text
       ↓
Convert text to lowercase
       ↓
Extract individual words
       ↓
Remove stop words
       ↓
Calculate word frequency
       ↓
Rank important keywords
       ↓
Compare words with topic dictionary
       ↓
Detect possible topics
       ↓
Generate keyword cloud
       ↓
Display analysis
       ↓
Save recent analysis
```

---

## 🔑 Keyword Extraction

The application first separates the text into individual words.

For example:

```text
Artificial intelligence is changing technology.
```

After removing common words:

```text
artificial
intelligence
changing
technology
```

These words are then counted and ranked according to their frequency.

---

## 🚫 Stop Words

Common words that usually provide little information are removed during keyword extraction.

Examples:

```text
the
is
a
an
and
or
of
to
in
on
for
with
this
that
it
are
was
were
```

This allows the application to focus on more meaningful words.

---

## 📊 Keyword Frequency

Each meaningful word is assigned a frequency based on how many times it appears.

Example:

```text
AI technology is growing.
AI technology is changing technology.
```

Possible result:

```text
technology ×3
AI ×2
growing ×1
changing ×1
```

The most frequent words are displayed at the top of the keyword ranking.

---

## 🏷️ Topic Detection

The application uses a predefined topic dictionary.

Some supported topics include:

| Topic                      | Example Keywords                         |
| -------------------------- | ---------------------------------------- |
| 🤖 Artificial Intelligence | AI, machine, learning, neural, algorithm |
| 💻 Technology              | software, hardware, computer, digital    |
| 🎓 Education               | student, college, school, teacher, exam  |
| 💼 Business                | company, market, customer, sales         |
| 🏥 Healthcare              | health, hospital, doctor, patient        |
| 🌱 Environment             | climate, pollution, recycling, energy    |
| 👨‍💻 Programming          | coding, Python, Java, JavaScript         |
| ☁️ Cloud Computing         | AWS, cloud, server, deployment           |
| 🔐 Cybersecurity           | security, password, encryption, malware  |
| 🚀 Space                   | astronaut, NASA, planet, rocket          |

If multiple keywords from a topic are found, that topic can be detected.

---

## ☁️ Keyword Cloud

The application generates a simple keyword cloud.

Frequently occurring words are displayed using larger text.

Example:

```text
          technology

     AI          programming

          machine learning

       education
```

The font size is based on keyword frequency.

---

## 📈 Analysis Dashboard

The dashboard provides:

* Total words
* Unique words
* Number of extracted keywords
* Number of detected topics

Example:

```text
Total Words      50
Unique Words     32
Keywords         10
Topics            3
```

---

## 💾 LocalStorage

The latest five analyses are stored in the browser.

Storage key:

```text
keywordTopicHistory
```

Each stored record contains:

* Original text
* Number of keywords
* Number of topics
* Analysis time

No external database is required.

---

## 📁 Project Structure

```text
KeywordTopicExtractor/
│
├── index.html
└── README.md
```

The complete application is contained inside one HTML file.

---

## 🚀 How to Run in VS Code

### Step 1 — Create Folder

Create a folder named:

```text
KeywordTopicExtractor
```

### Step 2 — Open in VS Code

Open the folder using Visual Studio Code.

### Step 3 — Create File

Create:

```text
index.html
```

### Step 4 — Add Code

Paste the complete Keyword & Topic Extractor code into `index.html`.

### Step 5 — Run

You can either:

* Open `index.html` directly in a browser, or
* Use the **Live Server** extension in VS Code.

### Step 6 — Test

Enter a paragraph and click:

```text
Extract Keywords
```

---

## 🧪 Sample Input

```text
Artificial intelligence and machine learning are transforming education and technology. Students are using AI applications to learn programming, develop software, and build innovative technology projects. Machine learning models and artificial intelligence tools are becoming important in modern education.
```

### Expected Topics

```text
🤖 Artificial Intelligence
💻 Technology
🎓 Education
👨‍💻 Programming
```

### Possible Keywords

```text
technology
artificial
intelligence
machine
learning
education
students
programming
software
applications
```

---

## 📋 Sample Test Cases

| Input                                           | Expected Topic |
| ----------------------------------------------- | -------------- |
| AI and machine learning are improving software. |                |
