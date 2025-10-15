AI Search Prompt Design – Dallas County, Texas


Overview

This project builds an AI-based news search system that collects and filters law-enforcement and true-crime stories from Dallas County, Texas.
It uses SerpApi to fetch Google News results, filters them by keywords, and exports a clean dataset for analysis.

Features

User inputs date range

Fetches Dallas-area news articles via SerpApi

Filters using keyword rules

Removes duplicates

Exports clean CSV file

Requirements

Python 3.12

Google Colab

Packages: google-search-results, pandas, requests, beautifulsoup4, tqdm

Setup in Google Colab

Install dependencies

!pip install google-search-results pandas requests beautifulsoup4 tqdm


Add SerpApi API key.

Run the notebook cells in order.

The filtered results are saved as

Dallas_County_LawEnforcement_<start>_to_<end>.csv

Filtering Rules

Filter-in keywords: police, officer, sheriff, arrest, deputy, body cam, investigation, drug trafficking, domestic violence.
Filter-out keywords: fatal shooting, deadly shooting, officer-involved shooting.

Output

CSV file with columns:

Article Title

Publication Date

Source/Outlet

Direct URL

Troubleshooting

If import errors occur, reinstall using:

!pip install --upgrade --force-reinstall google-search-results
