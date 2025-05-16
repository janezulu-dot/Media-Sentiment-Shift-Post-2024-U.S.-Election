# 🌍 GDELT Analysis: International Relations Shifts After the 2024 US Presidential Election

**Author:** Jane Zulu  
**Course:** BANA 6390 - Cloud Computing and AI  
**Instructor:** Dr. Herbert Remidez  
**Date:** April 1, 2025  

## 📌 Overview
This project analyzes shifts in global diplomatic behavior, media sentiment, and event patterns using the GDELT (Global Database of Events, Language, and Tone) dataset. The focus is on understanding how the 2024 U.S. presidential election — which resulted in Donald Trump's return to office — affected international relations.

## 🧠 Project Goals
- Detect statistically significant changes in international events and tone after the election.
- Visualize geopolitical response patterns using GDELT event codes.
- Interpret structural changes in global media narratives.

## 📊 Data Source
- **Dataset:** [GDELT Event Database](https://www.gdeltproject.org/data.html)
- **Period Analyzed:** October 1 – December 31, 2024  
- **Tools Used:** Google BigQuery, GCP Storage, SQL  
- **Events Analyzed:** Over 3 million, filtered to 2.1M pre-election and 923K post-election U.S.-related events.

## 🔑 Key Variables
- `EventCode`, `QuadClass`, `GoldsteinScale`, `AvgTone`
- `NumArticles`, `NumMentions`, `NumSources`
- `Actor1CountryCode`, `Actor2CountryCode`

## 🔍 Key Insights
- **Military Force Events** increased by 76.4% post-election.
- **Israel–Lebanon** saw the most improved diplomatic tone (+2.3 Goldstein).
- **North Korea–Russia** experienced the most deterioration (-1.4 Goldstein).
- **Media Narrative Shift**: Fewer unique sources post-election, indicating rising source concentration.
- **Geographic Attention Shift**: From Middle East to Eastern Europe and East Asia, even as sentiment in the Middle East improved.

## 🧼 Data Pipeline
- Data extracted from BigQuery public GDELT tables.
- Stored in GCP buckets and processed using SQL.
- Cleaned, filtered by date, and segmented by period (pre/post-election).

## 🧭 Future Work
- Explore model-based forecasting of diplomatic sentiment trends.
- Expand to cover multiple elections or longitudinal international events.
