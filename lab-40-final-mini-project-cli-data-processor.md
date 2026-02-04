# Lab 40: Final Mini-Project: Building a CLI Data Processor

## Objectives
- Learn how to fetch data from an API using a script.
- Understand how to save JSON data to a file.
- Implement command-line interface (CLI) arguments for file path or API URL.
- Integrate logging to monitor progress.
- Handle and manage exceptions in a Python program.
- Validate JSON data effectively.

## Prerequisites
- Basic understanding of Python programming.
- Familiarity with command-line interfaces.
- Access to an internet connection to fetch API data.
- Python 3.x installed on your system.

## Lab Tasks

### Task 1: Setting Up the Environment
**Install Required Packages:**
```bash
pip install requests
The requests library will be used to fetch data over HTTP from an API.

Create a Python File:

Create a new file named data_processor.py.

Task 2: Fetching Data from an API
Outline a Script to Fetch Data:

import requests
import json
import argparse
import logging
Define a Function to Fetch API Data:

def fetch_data(api_url):
    try:
        response = requests.get(api_url)
        response.raise_for_status()  # Check if the request was successful
        data = response.json()
        return data
    except requests.exceptions.HTTPError as http_err:
        logging.error(f"HTTP error occurred: {http_err}")
    except Exception as err:
        logging.error(f"Other error occurred: {err}")
This function takes an API URL, makes an HTTP GET request, and returns JSON data if successful.

Task 3: Saving JSON to a File
Create a Function to Save Data:

def save_data_to_file(data, file_path):
    try:
        with open(file_path, 'w') as json_file:
            json.dump(data, json_file, indent=4)
        logging.info(f"Data successfully saved to {file_path}")
    except Exception as e:
        logging.error(f"Error saving data: {e}")
JSON data is saved to a specified file path.

Task 4: Implementing CLI Arguments
Add CLI Argument Parsing:

def parse_arguments():
    parser = argparse.ArgumentParser(description='CLI Data Processor')
    parser.add_argument('--api_url', type=str, required=True, help='API URL to fetch data from')
    parser.add_argument('--file_path', type=str, required=True, help='Path to save JSON data')
    return parser.parse_args()
Task 5: Logging Progress
Set Up Logging:

logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
Logging will provide timestamped messages concerning the process status.

Task 6: Main Function Implementation
Combine All Parts:

if __name__ == '__main__':
    args = parse_arguments()
    logging.info("Started fetching data...")
    data = fetch_data(args.api_url)
    if data:
        save_data_to_file(data, args.file_path)
Task 7: Validating JSON Data
JSON validity is already confirmed using response.json() in fetch_data().

Conclusion
You have successfully built a CLI data processor in Python capable of:

Fetching data from an API.

Handling possible errors.

Logging progress.

Saving data to a file.

This mini-project demonstrates the integration of important Python modules like requests, argparse, and logging, giving you practical exposure to real-world data processing through a command-line interface.
