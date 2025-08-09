📊 College Event Feedback Analysis
This project analyzes student feedback from multiple college events to identify what attendees liked, areas for improvement, and overall satisfaction levels.
It uses Python, pandas, matplotlib, seaborn, WordCloud, and TextBlob for data cleaning, visualization, and sentiment analysis.

📌 Project Overview
College events often gather written feedback from attendees, but manually summarizing opinions can be time-consuming.
This analysis automates that process by:

Cleaning and preprocessing survey data

Performing sentiment analysis on feedback

Visualizing rating distribution & sentiments

Generating word clouds for likes and improvement suggestions

Summarizing key statistics and top suggestions

This helps organizers quickly understand attendees’ experience and make data-driven improvements for future events.

📂 Dataset
The dataset (feedback.csv) contains columns such as:

Column	Description
Event Name	Name of the event
Event Date	Date of the event
Overall Rating	Rating given by the attendee (1–5)
What did you like about the event?	Positive aspects shared
What could be improved?	Suggestions for improvement
Would you attend again?	Yes / No / Maybe
Any other comments?	Extra feedback
⚙️ Steps in the Analysis
1️⃣ Data Loading & Cleaning
Loaded the feedback CSV using pandas

Dropped rows with missing feedback in key comment fields

Reset index after cleaning

2️⃣ Sentiment Analysis
Used TextBlob to analyze polarity of answers to
"What did you like about the event?"

Classified feedback as Positive, Negative, or Neutral

3️⃣ Data Visualization
Event Rating Distribution — Count plot showing how attendees rated events

Sentiment Distribution — Visualization of positive/negative/neutral sentiments

Word Clouds:

For What Students Liked — Shows the most frequent positive words

For What Could Be Improved — Highlights common improvement requests

4️⃣ Summary Statistics
Sentiment Counts (Positive / Neutral / Negative)

Average Overall Rating across events

Top Suggestions for Improvement (most frequent)

📊 Example Insights (from sample run)
Average Rating: 3.5 / 5

Sentiment Distribution: Mostly positive feedback

Top Suggestions: Time management, more food options, better lighting, more water stations

What People Liked Most: Good organization, engaging performances, informative sessions

🛠️ Libraries Used
python
pandas
numpy
matplotlib
seaborn
wordcloud
textblob
You can install them via:

bash
pip install pandas numpy matplotlib seaborn wordcloud textblob
🚀 How to Run This Project
Clone the repository

bash
git clone <your-repo-url>
cd <repo-folder>
Install dependencies

bash
pip install -r requirements.txt
Run the Jupyter/Colab Notebook
Open and execute the notebook:

Load dataset

Run all cells to see visualizations and summary statistics

📌 Future Improvements
Add comparison charts between different events

Perform sentiment analysis on “What could be improved?” as well

Export results to PDF/Excel dashboard

Use NLP models (e.g., transformers) for deeper sentiment accuracy

📜 License
This project is open-source. You are free to use and adapt it for your own event analysis.
