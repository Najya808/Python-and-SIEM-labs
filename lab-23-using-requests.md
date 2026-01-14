What I Learned

In this lab, I learned how to perform HTTP requests in Python using the requests library. I practiced sending GET requests, inspecting HTTP response status codes, and parsing JSON responses. These skills are fundamental for interacting with RESTful APIs and retrieving web data programmatically.

 Lab Objectives

Understand how to perform HTTP requests using Python's requests library.

Retrieve and interpret HTTP response status codes.

Parse JSON data from HTTP responses.

Gain foundational knowledge of interacting with web APIs.

🧪 Lab Tasks Performed
🔹 Task 1: Setting Up the Environment

Install Requests Library

pip install requests


Import Requests Library

import requests

🔹 Task 2: Making a Basic HTTP GET Request

Send GET Request to GitHub API

response = requests.get("https://api.github.com")


Inspect the Status Code

print(response.status_code)


Explanation:

requests.get(url) sends an HTTP GET request.

response.status_code tells us the server's response:

200 → OK

404 → Not Found

500 → Internal Server Error

🔹 Task 3: Parsing JSON Response

Convert Response to JSON

response_data = response.json()
print(response_data)


Explanation:

response.json() parses JSON from the server into a Python dictionary.

You can now access specific data points, e.g., current API status or repository information.

Example:

# Print current GitHub API rate limit info
print(response_data.get('current_user_url'))

🧩 Key Concepts

HTTP Requests: Used to communicate with web servers and APIs.

Status Codes: Indicate request success or failure.

JSON Parsing: Converts API responses into Python-friendly dictionaries.

Requests Library: Simplifies making HTTP calls in Python.

 Summary

By completing this lab, I can now:

Install and import Python libraries.

Execute HTTP GET requests to APIs.

Interpret HTTP status codes.

Parse and use JSON data from API responses.

These skills are foundational for building web-integrated applications, fetching live data, and working with RESTful APIs.
