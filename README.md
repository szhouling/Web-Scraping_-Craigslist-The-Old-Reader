# Web Scraping and Automation Project

## Overview

This project involves web scraping and automation tasks using Python. The goal is to scrape item listings from the "free" category on Craigslist in the San Francisco Bay Area, save the HTML content of these listings to disk, and then parse specific details from the saved HTML files. Additionally, the project includes automating the login process for The Old Reader website.

## Part 1: Scraping and Saving HTML Content from Craigslist

### Target Identification

- Navigate to the Craigslist "free" section in the San Francisco Bay Area.
- Interact with page sorting and pagination to understand how listings are organized.

### Fetching Listing URLs

- Use `requests` and `BeautifulSoup` to extract listing URLs.
- Identify the structure holding the links and retrieve the URLs for the first 250 unique listings.

### Saving HTML Pages

- Fetch each listing's HTML content and save it to a separate file on disk.
- Organize files using the listing ID for easy identification.

## Part 2: Parsing and Displaying Information from Saved HTML

### Reading Saved HTML Files

- Write a script to read each saved HTML file from disk.

### Extracting Information

- Use `BeautifulSoup` to parse HTML content.
- Extract details like title, image URL, description, post ID, posted date, and last updated date.

## Part 3: Automating Login on The Old Reader

### Creating and Verifying The Old Reader Account

- Create an account on The Old Reader and verify manual login.

### Exploring the Login Mechanism

- Inspect the login form and identify crucial `<input>` fields.

### Analyzing Network Traffic for Login Request

- Understand the network request made during login and the payload sent to the server.

### Automating the Login Process

- Use Python with `requests` to simulate the login process.
- Maintain login state with a session object and send a POST request to the login form's action URL.

### Verifying Successful Login

- Check cookies in the session object to confirm successful login.

