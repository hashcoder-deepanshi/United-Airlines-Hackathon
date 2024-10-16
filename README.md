# United-Airlines-Hackathon

This project focuses on analyzing call center data to identify recurring issues that can be resolved using self-service options in the Interactive Voice Response (IVR) system. The goal is to reduce unnecessary agent intervention, improve efficiency, and enhance customer satisfaction. The project utilizes call transcripts, call reasons, sentiment data, and customer data to uncover insights and propose actionable recommendations for IVR improvements.

## Link to our PPT
[View PPT](https://www.canva.com/design/DAGTFNl5GxA/dM0xhHY7_rl3gPyDjLperw/edit?utm_content=DAGTFNl5GxA&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

# Key Objectives:
1. Data Preprocessing: Clean and merge data from multiple CSV files to create a consolidated dataset for analysis.
2. Call Transcript Analysis: Use Natural Language Processing (NLP) techniques to extract keywords from call transcripts and identify recurring issues.
3. Call Reason Analysis: Examine call reasons to identify common issues and trends.
4. IVR System Improvement Recommendations: Propose enhancements to the IVR system based on the insights from data analysis.
5. Data Visualization: Generate insightful visualizations such as word clouds, bar plots, and box plots to represent key findings.

# Data Preprocessing

## Files Used:
* calls.csv: Contains call metadata such as call ID, agent ID, call start/end times, and transcripts.
* customers.csv: Includes customer details such as customer_id and elite_level_code.
* reason.csv: Contains primary reasons for each call.
* sentiment_statistics.csv: Provides sentiment analysis of agent and customer tones during calls.

## Key Steps:
1. Merging Data: Merged all relevant datasets (calls, customers, reasons, and sentiments) based on common identifiers like call_id and customer_id.
2. Cleaning Data: Removed unwanted columns, handled missing values, and cleaned the call_transcript field by removing irrelevant comments and common stop words.
3. Handling Outliers: Box plots were used to identify and remove outliers in fields like handle_time.

# Call Transcript Analysis
We performed Natural Language Processing (NLP) on the call_transcript field to identify recurring issues that could have been handled via the IVR system. Using CountVectorizer, we extracted the top keywords from the cleaned transcripts to uncover patterns in customer queries.

# Usage

1. Clone the repository:

```
git clone [https://github.com/your-username/call-center-analysis.git](https://github.com/hashcoder-deepanshi/United-Airlines-Hackathon)
```
# Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request to improve the analysis or suggest new features.

# Future Improvements
* Enhance the NLP pipeline by incorporating more sophisticated models like spaCy or BERT.
* Add sentiment analysis for better understanding of customer and agent interactions.
* Implement time-series analysis to study patterns over specific periods (e.g., peak hours, seasonal trends).
