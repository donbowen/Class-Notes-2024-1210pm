## Planning my solution for the midterm 

Question: Is positive or negative sentiment associated with better or worse stock returns

Methods: Natural Language Processing (NLP) / textual analysis, cross-sectional event study, scraping

Rough steps:

1. Which firms?
2. Download 10-Ks from SEC Edgar 
3. Measure sentiment from text
4. Download returns "around" the 10-K. And convert to CARs.
5. Add the return data to my sample
6. ANALYSIS 

Dataset I want:
- Firm-event level
- Variables: sentiment of the 10k (maybe several versions), CAR (maybe several versions)

Prompts 3 Qs:
1. Which firms? --> S&P500. Drawback: Only large firms. Adv: Easier to digest (hard drive space). 
2. How to get return vars?  (Answered)
3. How to get sentiment measures?

Divide the project into X files:
1. Download text files (get tickers, get 10-ks)
2. Build sample
   - get returns
   - get account vars
   - merge all data we want
   - EDA, etc.
3. messy_analysis 
4. analysis_report


What: Download the 10-K closest to but before Mar 1 2020 for MSFT, AMZN, and AAPL. Don't "brute force" it - meaning don't type dl.get() multiple times. If you can, incorporate the tips on how to build a spyder from the website.