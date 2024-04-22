# Google Spider

This is a Scrapy spider designed to scrape business listings from Google search results.

## Description

This spider retrieves information such as business name, address, phone number, hours of operation, website, rating, and reviews from Google search results based on provided keywords. It utilizes Scrapy for web scraping and can handle dynamic content rendering.

## Prerequisites

Before you run this spider, ensure you have the following installed:

- Python (>=3.6)
- Scrapy
- `csv` module
- `urllib.parse`
- `re` module

## Installation

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/Muhammadsheraz492/get_data_from_google.git
    ```

2. Navigate to the project directory:

    ```bash
    cd google_doc
    ```

3. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Prepare your input data:
   
   - Ensure you have a CSV file named `keywords_aus.csv` with a column named `keywords` containing the search keywords.

2. Run the spider:

    ```bash
    scrapy crawl amazon_server_script_3
    ```

    Alternatively, you can run it with logging to a file:

    ```bash
    scrapy crawl amazon_server_script_3 -o output.csv
    ```

## Configuration

- The spider is configured to use `utf-8-sig` encoding for reading CSV files. If your CSV files have a different encoding, modify the `read_csv` function accordingly.
- You can adjust the spider settings such as `CONCURRENT_REQUESTS`, `RETRY_TIMES`, and `DOWNLOAD_DELAY` in the `custom_settings` dictionary within the spider class.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT](LICENSE)
