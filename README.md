# Sportsbook-Probability

Over the past few months, I built an end-to-end machine learning pipeline to predict NBA game outcomes using real betting odds, advanced metrics, and game history data — then tested it with a bankroll strategy using the Half Kelly Criterion. 



This project helped me exercise my skills in data engineering, feature selection, model tuning, and statistical analysis, but also helped me to install a cost-benefit strategy that individuals could use for financial risk management. 



Since the repeal of PASPA in 2018, sports betting has gained mainstream acceptance, and become influential to our current tech-driven society. However, this activity can lead to varying levels of financial insecurity if left unmanaged. With my current knowledge of where the wealth gap is today, I wanted to create a system that allows sports betting to remain a fun activity without being a potential bottleneck to a person’s financial security. 



Here’s what I built:

	•	A fully merged dataset combining:

	•	Betting odds (OddsAPI)

	•	Game history & Team Stats Per Game (Basketball Reference)

	•	Advanced metrics like Offensive/Defensive Rating, Adjusted Net Rating, Effective Possession Ratio (TeamRankings)

	•	A Gradient Boosting model to predict game outcomes

	•	A bankroll management simulation that used the Half Kelly Criterion to calculate optimal bet sizes

	•	An interpretable output format showing team matchups, betting edges, and predicted win probabilities



Challenges I overcame:

	•	Data Source availability: Most established sources are hidden behind a paywall, so I web scraped from multiple databases in order to cast a wide enough net for the model to train and learn relationships between data points. 

	•	Missing time/date columns: most of the files didn’t have game IDs or timestamps, so I cleaned and aligned Team names to enable accurate merging. 

	•	Duplication risk: I validated merges to preserve one row per game

	•	Feature engineering: I created structured metrics for offensive/defensive performance over games for every home and away stint for each team. 



Key results:

	•	Model accuracy improved significantly over baseline (up to 67% on test data). 

	•	The model highlighted offensive rating, adjusted net rating, win percentage, home free throw attempts, away turnovers, and away rebounds having high significance on the presence of a home victory occurring. 

	•	A conservative betting strategy using Half Kelly produced sustainable bankroll growth across simulated matchups
