# Rev⭐Scrap - Reviews Scraper Tool
Website that scrapes Google for reviews of an item (product, movie, etc.) and runs sentiment analysis on the results.

Check out [live]()!

Note: For best results ensure to enter specific product name and not generic.

## What it uses
 - *Huggingface* for performing sentiment analysis on the reviews
    - Uses `LiYuan/amazon-review-sentiment-analysis` for 1-5 star rating.
    - Uses `cardiffnlp/twitter-roberta-base-sentiment-latest` for positive/neutral/negative sentiment.
 - *Apify* for scraping reviews from Google.
 - *Streamlit* for hosting the website.
 - *WordCloud* for creating word clouds.

## You can host locally by following the steps given below:
1. Install requirements
```
pip install -r requirements.txt
```
3. Make an account on [Apify](https://apify.com/)
4. Add your API token from apify to `/.streamlit/secrets.toml` :
```
APIFY_TOKEN='YOUR_API_TOKEN'
```
2. Finally run `main.py`
```
streamlit run main.py
```

## References
 - Inspired by [nus-sentiment](https://github.com/nus-sentiment/nus-sentiment)
