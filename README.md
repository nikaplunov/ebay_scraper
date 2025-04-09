# eBay Gift Card Auction Scraper

🔍 A Python project designed to collect live auction data for gift cards listed on eBay, utilizing the eBay Browse API and OAuth authentication. This tool facilitates market analysis by examining price dispersion, liquidity, and bidding behaviors over time.

## Project Overview

Gift cards have become a significant component of consumer spending, often regarded as cash equivalents due to their direct monetary value. Understanding their secondary market dynamics, especially on platforms like eBay, provides valuable insights into consumer behavior and market efficiency. This project aims to shed light on these aspects by systematically collecting and analyzing auction data.

## Features

- **Comprehensive Data Collection**: Gathers live auction listings for gift cards within eBay's Gift Cards category (Category ID: 172008).
- **Detailed Information Extraction**: Captures essential details including:
  - Seller's username and feedback score
  - Item ID and title
  - Extracted gift card value from the title
  - Current bid amount and bid count
  - Shipping cost
  - Auction end time
  - Item condition
  - Direct URL to the listing
- **Pagination Handling**: Automatically navigates through all available auction pages to ensure complete data retrieval.
- **Data Storage**: Saves the aggregated data into a structured CSV file (`ebay_gift_card_auctions.csv`) for subsequent analysis.

## Setup Instructions

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/nikaplunov/ebay_scraper.git
   cd ebay_scraper
   ```

2. **Obtain eBay OAuth Token**:
   - Register for the [eBay Developer Program](https://developer.ebay.com/).
   - Create an application to generate your OAuth access token.

3. **Configure API Credentials**:
   - Replace `"Your OAuth TOKEN"` in the script with your obtained OAuth access token.


## Research Objectives

This project is designed to facilitate research into several key areas:

- **Price Dispersion Analysis**: Investigate how gift cards, despite being cash equivalents, exhibit varying price points in secondary markets. Jennifer Pate Offenberg's study, ["Markets: Gift Cards"](https://www.aeaweb.org/articles?id=10.1257/jep.21.2.227), provides foundational insights into this phenomenon.

- **Market Liquidity Examination**: Assess the ease with which gift cards from different retailers are sold in secondary markets and how this liquidity impacts their pricing.

- **Bidding Behavior Insights**: Analyze patterns such as auction sniping and the effect of seller reputation on final sale prices.

These objectives build upon existing literature, including the work by Lesley Chiou and Jennifer Pate titled ["Internet Auctions and Frictionless Commerce: Evidence from the Retail Gift Card Market"](https://ideas.repec.org/a/kap/revind/v36y2010i3p295-304.html), which explores online auction dynamics for gift cards.

