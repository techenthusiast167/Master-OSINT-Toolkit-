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

- Verify the accuracy of email addresses and provide relevant information about them

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

> pip install requests beautifulsoup4 waybackpy spacy phonenumbers exifread tldextract python-whois dnspython
python -m spacy download en_core_web_sm



# Save the toolkit script:

**Open Nano**

> nano master_osint.py

Copy the tool script via the link https://gist.github.com/techenthusiast167/a95ce477eac6eb1b0db9f22b3a55ca2c and paste it into the nano editor, save by pressing **(Ctrl+O), and exit (Ctrl+X)**.




**Tips**:

Use python -m pip install package-name if pip is not recognized.

Always activate your virtual environment before installing libraries.

Fix missing modules using pip install [package_name] as needed.
Usage



# Running the tool:

**Note: Before ruining the tool, prepare input files**:

For the **Website Metadata and Entity Scraper**, create a file named **urls.txt** in the same directory, containing one **URL per line**. This will facilitate automating the extraction of results using the **Number Ten module**.

**Run the tool**:

> python3 master_osint.py


- You will see a colorized logo and a menu with multiple investigative modules numbered 1 through 13.

- Select a module by entering its associated number when prompted.
  
- Follow any on-screen instructions to input required data (e.g., **image path, username, email address, domain, phone number**, etc).




# Module Descriptions


1. **Image Geolocation**: Extract GPS data from image EXIF or perform manual location guidance.

2. **Social Media Investigation**: Generate profile URLs on 30+ popular platforms by username.
   
3. **Email Analysis**: Detect breach status and search public pastes and Google for emails.
   
4. **Email Lookup & Verification**: Verify email data via Hunter.io and other services.
   
5. **Domain Investigation**: Retrieve WHOIS info, DNS records, and subdomain enumeration.
   
6. **Metadata Extraction**: Extract EXIF metadata and file system information from files.
   
7. **Google Dorking**: Perform advanced Google searches using powerful operators.
   
8. **Wayback Machine Lookup**: Access archived webpage snapshots.
   
9. **IP Geolocation & Blacklist Checking**: Locate IP geolocation and check abuse blacklists.
    
10. **Website Metadata & Entity Scraper**: Scrape website metadata and extract named entities using NLP.
    
11. **Phone Number Investigation**: Validate phone numbers and generate OSINT search dorks.
    
12. **Reverse Image Search**: Query multiple reverse image search engines for investigation.

13. **Exit**: Safely exit the toolkit.



# API Keys Setup

**Several modules require API keys for full functionality. Replace placeholder keys in the script**:


- **HaveIBeenPwned API** (for Email breach checks

- Register at HaveIBeenPwned API and replace YOUR_API_KEY placeholder correctly where is required in the script: https://haveibeenpwned.com/api/v3

- **Your HUNTER_IO API KEY** - for Hunter.io email verification.

- Sign up to create a free account at Hunter.io and replace your API KEY placeholder correctly where required in the script: https://hunter.io/

- **AbuseIPDB API** (for IP blacklist checks)
  
Register at AbuseIPDB and replace the API key placeholder correctly where needed in the script: https://www.abuseipdb.com 


**Security Note**: Never hardcode API keys in public repositories. Use environment variables or config files instead.


# Ethical Considerations

Use this tool responsibly for legal and educational research only.
Obtain consent before investigating third-party data.

Do not use for any illegal purposes or to infringe on privacy.

Comply with the terms of service of all websites and APIs involved.
Contact & Support


**Contributing**:

Feel free to submit issues, and create pull requests to improve or extend this toolkit.

**For support, feedback, or contributions, you can connect with me via**:

Email: preciousvincentct@gmail.com

LinkedIn: http://linkedin.com/in/tech-enthusiast-669279263


# MASTER OSINT v2

A breakdown of the newly built version: https://x.com/ctprecious/status/1947949365957685464?s=46
