MASTER OSINT - Beginner Friendly Open Source Intelligence Toolkit

Master OSINT is a comprehensive, beginner-friendly Python toolkit designed for open source intelligence investigations. The tool supports multiple investigative methods including image geolocation, social media profiling, email breach checks, domain lookup, metadata extraction, Google dorking, Wayback Machine querying, IP geolocation with blacklist checks, reverse image search, and phone number validation.

# Table of Contents

- Features

- Prerequisites

- Installation on Kali Linux

- Usage

- Module Descriptions

- API Keys Setup

- Ethical Considerations

- Contact & Support


# Features

- Extract GPS coordinates from image EXIF data

- Generate social media profile URLs based on username

- Check if email addresses have been breached using HaveIBeenPwned API

- Perform domain WHOIS lookups including registrar, domain age information and subdomain enumeration 

- Extract metadata from documents and images

- Perform Google Dorking queries for sensitive information discovery

- Retrieve historical snapshots of URLs via the Wayback Machine

- Geolocate IP addresses and check blacklists (AbuseIPDB)

- Scrape website metadata and extract emails, names, locations

- Validate phone numbers, retrieve country, carrier, and type information; search OSINT dorks for in-depth investigations on phone number 

- Make a quick investigation by verifying image authenticity and valuable information 


# Prerequisites

**Ensure your Kali Linux system has the following**:

- Python 3.x

- pip package manager

- Internet connection for API calls and web lookups

- Installation on Kali Linux

# Update system packages:

> sudo apt update

# Create and activate a Python virtual environment:

> virtual my_temp_venv

> source my_temp_venv/bin/activate

# Install the required Python packages:

**You can install all dependencies at once**:

> pip install requests exifread waybackpy beautifulsoup4 tldextract python-whois spacy phonenumbers
python -m spacy download en_core_web_sm

# Save the toolkit script:

**Open Nano**

> nano master_osint.py

Copy the tool script via the link https://gist.github.com/techenthusiast167/8e37f06df91c07bd5bb774831ab53e75 and paste it into the nano editor, save by pressing **(Ctrl+O), and exit (Ctrl+X)**.

**Verify with**:

> ls

**Tips**:

Use python -m pip install package-name if pip is not recognized.

Always activate your virtual environment before installing libraries.

Fix missing modules using pip install [package_name] as needed.
Usage

# Run the tool with:

> python3 master_osint.py

You will see a colorized logo and a menu with multiple investigative modules numbered 1 through 11.

Enter the number of the module you want to perform, and follow the prompts for inputs.

The tool may display results directly or open relevant web pages for further exploration.

Select option 12 at any time to exit gracefully.

# Module Descriptions

1. Image Geolocation: Extract GPS coordinates from image EXIF metadata

2. Social Media Investigation: Generate social media profile URLs from a given username

3. Email Analysis: Check if email has been breached (HaveIBeenPwned API) and Pastebin search

4. Domain Investigation: Perform WHOIS lookup and display domain age

5. Metadata Extraction: Extract metadata from documents or images

6. Google Dorking: Input custom Google dorks for sensitive info discovery

7. Wayback Machine Lookup: Fetch historical snapshots of URLs from Internet Archive

8. IP Geolocation & Blacklist: Geolocate IP addresses and check AbuseIPDB blacklist status

9. Website Metadata & Scraper: Extract meta tags, emails, names, and locations from websites

10. Phone Number Investigation: Validate phone number, retrieve country/carrier/type info, and search OSINT dorks

11. Reverse Image Search: Make a quick investigation of an image authenticity 

12. Exit the tool


# API Keys Setup

**Some modules require API keys**:

HaveIBeenPwned API (for Email breach checks: https://haveibeenpwned.com/api/v3 

Register at HaveIBeenPwned API and replace YOUR_API_KEY placeholder rightly where is required in the script.

AbuseIPDB API (for IP blacklist checks)
Register at AbuseIPDB and replace the API key placeholder rightly where needed in the script: https://www.abuseipdb.com 

Security Note: Never hardcode API keys in public repositories. Use environment variables or config files instead.


# Ethical Considerations

Use this tool responsibly for legal and educational research only.
Obtain consent before investigating third-party data.

Do not use for any illegal purposes or to infringe on privacy.

Comply with the terms of service of all websites and APIs involved.
Contact & Support


**For support, feedback, or contributions, connect with the creator**:

Email: preciousvincentct@gmail.com

LinkedIn: http://linkedin.com/in/tech-enthusiast-669279263
