# Research Pulse — arXiv Scientific Acceleration Dashboard

A **Python + Power BI** project exploring the growth and evolution of AI research using millions of arXiv papers. The project covers data collection, cleaning, feature extraction, analytical modelling and interactive visualisation.

## 📊 Dataset

The raw arXiv dataset is not included due to its size. You can download the dataset arxiv-metadata-oai-snapshot.json from the internet. This dataset has been mirrored on several websites, so download whichever one you like.

The project starts with a **3.16M-paper, ~5.3 GB arXiv metadata dataset**, covering 2007–2026. This dataset has got papers from every field of science, so I scoped them for my project context. I focused on seven AI related categories:

`cs.AI` · `cs.LG` · `cs.CL` · `cs.CV` · `stat.ML` · `cs.RO` · `cs.NE`

## 🔧 Data Pipeline

The pipeline processes the 3.16M-paper arXiv metadata dataset, scopes it to seven AI-related categories, extracts authors and category relationships, derives custom research-area tags, and prepares the final analytical model for Power BI. And the final scoped dataset contains **643K+ papers**.


## 🛠️ Tech Stack

- **Python:** Pandas, NumPy, Regex
- **Jupyter Notebook:** Data collection & preprocessing
- **Power BI:** Data modelling, DAX & visualisation
- **Deneb:** Custom Power BI visuals

## 📁 Files

```text
├── arxiv_data_pipeline.ipynb
├── Arxiv_Pulse_Report.pbix
└── README.md
```

## 📈 Dashboard Visuals

The dashboard covers **research growth, category trends, emerging subfields, cross-category relationships, author activity and collaboration patterns**, with interactive filtering across the report.

### Page 1 — Scientific Acceleration

- **Research Volume Trend:** Tracks the growth of AI research publications over time.
- **Category Composition:** Shows how the share of research across the seven AI categories has changed over the years.
- **Category Co-occurrence Matrix:** Highlights how frequently different research categories overlap within the same papers.
- **Monthly Research Trend:** Shows the monthly publication pattern and overall research activity.
- **Key Metrics:** Summarises total papers, 2026 YTD papers, average authors per paper, cross-category research rate and post-ChatGPT research volume

### Page 2 — Emerging Subfields & Collaboration

- **Subfield Rank Evolution:** Tracks how the popularity of emerging AI subfields has changed over time.
- **Subfield Similarity Matrix:** Shows the strength of relationships and overlap between emerging research areas.
- **Author Analytics Table:** Explores author publication volume, growth, multi-subfield involvement and collaboration.

## 🎯 Goal

The goal was to identify whether the papers in the AI filed ha increased in the past few years, and if so, what is the trend after ChatGPT was introduced, as LLMs have fast tracked the research process. This project successfully confirms that notion.
