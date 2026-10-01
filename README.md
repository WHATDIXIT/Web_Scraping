# Apna Job Scraper - Lucknow

A Python web scraping project that collects job listings from Apna's Lucknow jobs portal using **Requests** and **BeautifulSoup**.

## Features

* Scrapes job listings from multiple pages.
* Extracts company name, job title, location, work type and job type.
* Uses Pandas to organize the scraped data.
* Exports the collected data as a CSV dataset.

## Technologies Used

* Python
* Requests
* BeautifulSoup
* Pandas
* Google Colab / Jupyter Notebook

## Project Workflow

1. Send HTTP requests to Apna job listing pages.
2. Parse the HTML using BeautifulSoup.
3. Locate individual job cards.
4. Extract relevant job information.
5. Store the data in a Pandas DataFrame.
6. Export the final dataset to CSV.

## Dataset

| Column         | Description                                                             |
| -------------- | ----------------------------------------------------------------------- |
| `Company_Name` | Name of the hiring company                                              |
| `Job`          | Job title                                                               |
| `Place`        | Job location                                                            |
| `Work_Type`    | Work arrangement such as Work from Home, Work from Office, or Field Job |
| `Job_Type`     | Full Time or Part Time                                                  |

## Output

The dataset can be exported with:

```python
final.to_csv('apna_jobs_lucknow.csv', index=False)
```

`index=False` prevents the Pandas DataFrame index from being added as an extra CSV column.

## How to Run

Open the notebook in Google Colab or Jupyter Notebook and run the cells sequentially.

Install the required packages if needed:

```bash
pip install requests beautifulsoup4 pandas lxml
```

Then run the scraper and export the resulting DataFrame to CSV.

## Dataset

The scraped dataset is also available on Kaggle.

[View Dataset on Kaggle](https://www.kaggle.com/datasets/utkarshdixit050/lucknow-jobs)

| Column | Description |
|---|---|
| `Company_Name` | Name of the hiring company |
| `Job` | Job title |
| `Place` | Job location |
| `Work_Type` | Work arrangement such as Work from Home, Work from Office, or Field Job |
| `Job_Type` | Full Time or Part Time |

## Project Purpose

This project was created as a hands-on practice project for Python web scraping, HTML parsing, data collection, and data preprocessing using job listing data.

## Disclaimer

This project is intended for educational and practice purposes. Respect the website's terms of service, robots.txt, rate limits, and applicable laws when scraping websites.
