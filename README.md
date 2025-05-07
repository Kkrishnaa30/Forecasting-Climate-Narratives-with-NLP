# 🌍 Forecasting Climate Narratives Using NLP  
### A Multi-Source Analysis of Global Climate Change Discourse (2015–2025)

## 🔬 Project Overview  
This project introduces a comprehensive **Natural Language Processing (NLP)** framework to explore how public and scientific narratives surrounding **climate change** have evolved over the past decade. It analyzes over **10,000 climate-related articles** sourced from global news outlets and scientific journals to extract patterns in **sentiment**, **topic evolution**, and **thematic focus** using state-of-the-art NLP models.  

Rather than forecasting physical environmental metrics, the aim here is to **"forecast climate narratives"**—understanding what people are talking about, how their emotions and concerns change, and what themes are gaining or losing attention in global discourse. This allows for early detection of emerging concerns, shifts in public focus, and signals relevant for policy and communication strategies.

## 📊 Key Methodologies and Tools  

### 🗞️ 1. Data Collection  
- Articles scraped from sources including **Nature Climate Change**, **The New York Times**, **environment.org**, and Indian climate-focused platforms.  
- Extracted full text, titles, publication dates, and source metadata.  
- Time span: Articles published between **2015 and 2025**.

### 🧹 2. Text Preprocessing  
- Cleaned the dataset using techniques like:
  - HTML tag removal  
  - Tokenization  
  - Lemmatization  
  - Stop word filtering and lowercasing  
- Prepared the corpus for advanced NLP analysis using spaCy and NLTK.

### 😊 3. Sentiment Analysis  
- **VADER** was used for short texts like headlines, capturing sharp emotional spikes during major climate events.  
- **BERT (Bidirectional Encoder Representations from Transformers)** was fine-tuned for sentiment classification of long articles and scientific pieces, capturing nuanced tone.  
- Findings revealed:
  - Negative sentiment peaks after major natural disasters (e.g., Australian wildfires, Indian floods).
  - Positive sentiment rose after COP summits and green tech announcements.
  - A growing bifurcation between concern (disaster, inaction) and optimism (innovation, policy wins).

### 🧠 4. Topic Modeling with BERTopic  
- **BERTopic** was employed to detect and trace themes over time:
  - Uses transformer-based embeddings, UMAP for dimensionality reduction, and HDBSCAN for clustering.
  - Automatically labeled over **25 dominant climate-related topics**.
- Topic trends included:
  - 📉 *Carbon Emissions*, 🌿 *Renewable Energy*, 🛑 *Policy Inaction*, 🌊 *Flood Impact*
  - Regional differences showed South Asia discussing food/agriculture loss, while the U.S. focused on legislation and innovation.
  - Thematic spikes aligned with real-world events (e.g., post-COP26 rise in “Net-Zero” discussions).

### ✂️ 5. Summarization with Flan-T5  
- Used **Flan-T5**, a Google-developed transformer model, for extractive and abstractive summarization.
- Compressed long articles by over **78%** while preserving core meaning and sentiment.
- These summaries enhanced:
  - Topic clustering accuracy  
  - Time-series alignment of themes  
  - Identification of high-risk signals (e.g., repeated mentions of "record heatwave" or "policy inertia")

## 🔍 Key Findings and Insights  

### 📈 Sentiment Shifts  
- The emotional tone of climate narratives is **not static**—it fluctuates in response to:
  - Scientific breakthroughs  
  - Policy changes (like Paris Agreement commitments)  
  - Natural disasters and humanitarian crises  
- NLP analysis provided **early warnings** of rising concern, making this valuable for policy forecasting and public outreach.

### 🧩 Topic Dynamics  
- Topics like **Climate Justice**, **Climate Finance**, and **Carbon Neutrality** gained traction after 2020.
- **Seasonal trends** were observed: wildfire discussions peaked mid-year; flood-related discourse surged during monsoons.
- BERTopic revealed **policy-specific sentiment clusters**, allowing identification of public resistance or support on certain issues.

### 💡 Multi-Modal Narrative Intelligence  
- Although the study focused only on NLP, combining **summarization**, **sentiment**, and **topic modeling** allowed for narrative forecasting:
  - Predict which themes might dominate future climate discourse  
  - Detect misinformation patterns or regions with disengaged public sentiment  
  - Aid NGOs and governments in tailoring their messaging strategies

## 🧠 Implications  
This NLP pipeline can serve as a **decision-support system** for:
- **Policymakers**, by identifying shifting public opinion and emerging concerns  
- **Researchers**, by mapping the trajectory of climate-related discussion  
- **Media outlets**, by detecting oversaturation or narrative gaps in climate reporting  
- **Educators and advocates**, to design timely and data-backed campaigns

## 🛠️ Tools & Libraries Used  
- Python, Pandas, BeautifulSoup, Matplotlib  
- HuggingFace Transformers (BERT, Flan-T5)  
- **VADER** for rule-based sentiment analysis  
- **BERTopic**, UMAP, and HDBSCAN for topic modeling  
- NLTK, spaCy for preprocessing  

## 📚 Citation  
**Krishna Khandelwal, Arup Das, Jiacun Wang**  
*Forecasting Climate Trends: A Multi-Source Analysis of Global Climate Change Using NLP, Topic Modeling, and Summarization (2025)*
