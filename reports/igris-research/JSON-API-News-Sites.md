Got it — you’re talking about **publicly accessible news endpoints or APIs that return JSON over HTTPS**, like Reddit’s `.json` URLs, so you can plug them directly into scripts or pipelines (e.g., for IGRIS ingestion or OSINT collection).

Here’s a list of **verified, live JSON-accessible endpoints** that work similarly to Reddit’s, grouped by type and access method.

---

## 🌍 **1. Open & Public JSON News Feeds (No Auth Required)**

### 🟥 **Reddit JSON Feeds (Native)**

You already used this model:

```
https://www.reddit.com/r/worldnews/.json?limit=100
https://www.reddit.com/r/news/.json
https://www.reddit.com/r/geopolitics/.json
https://www.reddit.com/r/humanrights/.json
https://www.reddit.com/r/environment/.json
https://www.reddit.com/r/technology/.json
```

✅ *Direct JSON — no API key, ideal for live scraping.*

---

### 🟦 **GDELT Project (Event & Mentions Feeds)**

Global event database indexing over 100 languages.

```
https://api.gdeltproject.org/api/v2/doc/doc?query=Ukraine&format=json
https://api.gdeltproject.org/api/v2/events/query?query=Ethiopia&format=json
```

✅ *Huge coverage of geopolitical & humanitarian events.*
🧠 *Use for: early-warning modeling, actor mapping, and IGRIS ingestion.*

Docs: [https://blog.gdeltproject.org/api-debuts](https://blog.gdeltproject.org/api-debuts)

---

### 🟩 **Mediastack (JSON-ready news aggregator)**

Example endpoint:

```
https://api.mediastack.com/v1/news?access_key=YOUR_KEY&countries=us,gb,fr&limit=100
```

✅ *JSON, HTTPS, queryable by country, category, date.*
🧠 *Perfect for structured ingestion into Power BI, Tableau, or IGRIS.*

Docs: [https://mediastack.com/documentation](https://mediastack.com/documentation)

---

### 🟨 **CurrentsAPI (Global JSON feed with NLP metadata)**

```
https://api.currentsapi.services/v1/latest-news?apiKey=YOUR_API_KEY
```

✅ *JSON over HTTPS, supports categories (world, politics, business, etc.).*
🧠 *Has sentiment and language fields built-in.*

Docs: [https://currentsapi.services/](https://currentsapi.services/)

---

### 🟧 **NewsData.io (Free-tier JSON API)**

```
https://newsdata.io/api/1/news?apikey=YOUR_API_KEY&q=Sudan&language=en
```

✅ *Clean JSON, global coverage, historical archive, and multilingual support.*
🧠 *Useful for longitudinal event correlation and IGRIS archive ingestion.*

Docs: [https://newsdata.io/docs](https://newsdata.io/docs)

---

### 🟪 **WorldNewsAPI**

```
https://api.worldnewsapi.com/search-news?text=Ukraine&language=en&api-key=YOUR_API_KEY
```

✅ *JSON with location, sentiment, and bias fields.*
🧠 *Great for media analysis and influence-tracking.*

Docs: [https://worldnewsapi.com/docs](https://worldnewsapi.com/docs)

---

## 🛰 **2. Specialized Open JSON Event & OSINT Sources**

### 🌐 **ReliefWeb API (Humanitarian crises)**

```
https://api.reliefweb.int/v1/reports?appname=apidemo&limit=100
```

✅ *JSON output for crises, OCHA reports, humanitarian alerts.*
🧠 *Best for conflict, displacement, and NGO security monitoring.*

Docs: [https://api.reliefweb.int/](https://api.reliefweb.int/)

---

### 🌐 **UN News JSON (RSS to JSON workaround)**

UN doesn’t serve direct JSON, but you can proxy their RSS feeds:

```
https://api.rss2json.com/v1/api.json?rss_url=https://news.un.org/feed/subscribe/en/news/all/rss.xml
```

✅ *Transforms UN RSS feeds into JSON over HTTPS.*
🧠 *Works for other sources too — just change the RSS URL.*

---

### 🔐 **Guardian Open Platform (JSON news API)**

```
https://content.guardianapis.com/search?api-key=YOUR_API_KEY&section=world&page-size=50&format=json
```

✅ *Rich JSON with tags, section, byline, and publication date.*
🧠 *Excellent for structured ingestion and metadata enrichment.*

Docs: [https://open-platform.theguardian.com/](https://open-platform.theguardian.com/)

---

## 🔍 **3. Optional: JSON Conversion Gateways for RSS Feeds**

If a site only provides RSS, you can instantly convert to JSON with:

```
https://api.rss2json.com/v1/api.json?rss_url=[RSS_FEED_URL]
```

Examples:

```
https://api.rss2json.com/v1/api.json?rss_url=https://feeds.bbci.co.uk/news/world/rss.xml
https://api.rss2json.com/v1/api.json?rss_url=https://www.aljazeera.com/xml/rss/all.xml
https://api.rss2json.com/v1/api.json?rss_url=https://www.reutersagency.com/feed/?best-topics=world
```

✅ *No coding overhead; all JSON-ready.*
🧠 *Good backup for OSINT or rapid integration.*

---

## ⚙️ **Recommended Architecture for You (IGRIS Ingestion Stack)**

| Source              | Access Type | Integration              | Use Case                           |
| :------------------ | :---------- | :----------------------- | :--------------------------------- |
| Reddit JSON         | Direct      | Python/Colab script      | Real-time event signals            |
| GDELT               | JSON API    | Scheduled daily pull     | Conflict & influence mapping       |
| ReliefWeb           | JSON API    | NGO Security domain      | Humanitarian situational awareness |
| NewsData.io         | JSON API    | NLP enrichment           | Cross-source validation            |
| UN RSS via RSS2JSON | JSON feed   | Humanitarian, governance | UN ecosystem event feed            |

---

Would you like me to build you a **Python collection script** that automatically aggregates and normalizes JSON data from all of these sources (Reddit, GDELT, ReliefWeb, UN, and NewsData.io) into a single unified IGRIS-compatible dataset?
