## MASTER OSINT - An Advanced Open Source Intelligence Toolkit

Master OSINT is a comprehensive, beginner-friendly Python toolkit designed for open source intelligence investigations. The tool supports multiple investigative methods including image geolocation, social media profiling, email breach and verification checkup, domain lookup, metadata extraction, Google dorking, Wayback Machine querying, IP geolocation with blacklist checks, reverse image search, geospatial Intelligence and phone number validation.



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



- Extract GPS coordinates from images EXIF data.

- Investigate social media presence across 30+ platforms by username.

- Detect email breaches and dig through public pastes.

- Verify email validity using Hunter.io, ReverseContact.com, and Epieos.

- Perform WHOIS and DNS lookups, enumerate subdomains via crt.sh.

- Extract metadata from images/documents.

- Utilize Google advanced search operators (Google Dorking).

- Access archived website snapshots via Wayback Machine.

- Locate IP geolocation and retrieve abuse reports with AbuseIPDB.

- Scrape website metadata and extract named entities using spaCy NLP.

- Validate and investigate phone numbers with carrier and type information.

- Conduct reverse image searches using popular engines.

- Access powerful geospatial intelligence with Google Satellite & OpenStreetMap.


# Prerequisites

**Ensure your Kali Linux system has the following**:

- Python 3.x

- pip package manager

- Internet connection for API calls and web lookups

- Installation on Kali Linux

# Update system packages:


    sudo apt update


# Create and activate a Python virtual environment:


    virtual my_temp_venv

    source my_temp_venv/bin/activate



# Install the required Python packages:

**You can install all dependencies at once**:


    pip install requests beautifulsoup4 waybackpy spacy phonenumbers exifread tldextract python-whois dnspython
    python -m spacy download en_core_web_sm



# Save the toolkit script:

**Open Nano**

    nano master_osint.py

- **Copy the tool script via the link**:

**https://gist.github.com/techenthusiast167/a95ce477eac6eb1b0db9f22b3a55ca2c** 

**Master OSINT v2** and paste it into the nano editor, save it as **master_osint.py** by pressing **Ctrl+O, Enter, and Ctrl+X to exit**

**Master OSINT v3** is now out. You can get it via the link below:

**https://gist.github.com/techenthusiast167/5fb49b007d48cf2717bc3c12958e47b5**

- **Same installation as version2**


**Tips**:

Use python -m pip install package-name if pip is not recognized.

Always activate your virtual environment before installing libraries.

Fix missing modules using pip install [package_name] as needed.
Usage



# Running the tool:

**Note: Before ruining the tool, prepare input files**:

For the **Website Metadata and Entity Scraper**, create a file named **urls.txt** in the same directory, containing one **URL per line**. This will facilitate automating the extraction of results using the **number 10 module**.

**Run the tool**:

    python master_osint.py


You will see a menu with 14 OSINT modules plus an exit option. Enter the number of the module you want to run and follow the prompts.

**For example**:

- Enter a username to generate social media profile URLs.

- Enter an email to check breaches or verify validity.

- Enter domain names for WHOIS and DNS lookups.

- Provide image file paths for EXIF geolocation.

- Enter IP addresses for geolocation and blacklist checking.

- Use **urls.txt** file (one URL per line) in the folder for website metadata scraping.

- Results will print in the console or save to files depending on the module (e.g., metadata_output.json for website scraping).


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
   
13. **Geospatial Intelligence**: View any location coordinates or place using Google Satellite Maps and OpenStreetMap.

14. **Exit**: Safely exit the toolkit.



# API Keys Setup


**Some modules require API keys for full functionality**:

- **HaveIBeenPwned API key**: needed for email breach checks.
- Sign up at https://haveibeenpwned.com/API/Key and set your key in the script.

 - **Hunter.io API key**: needed for email verification.
 - Register at https://hunter.io and update the key in the script.

- **AbuseIPDB API key**: for IP blacklist checks.
- Register at https://www.abuseipdb.com/api and update accordingly.


Update the placeholder API key variables in master_osint.py with your keys to unlock full features.


**Security Note**: Never hardcode API keys in public repositories. Use environment variables or config files instead.

# Ethical Considerations

Use this tool responsibly for legal and educational research only.
Obtain consent before investigating third-party data.

Do not use for any illegal purposes or to infringe on privacy.

Comply with the terms of service of all websites and APIs involved.
Contact & Support


**Contributing**:

Contributions, suggestions, and bug reports are welcome! Please open an issue or submit a pull request.

**Contact**:

Follow me on LinkedIn for updates and future releases.

**LinkedIn**: http://linkedin.com/in/tech-enthusiast-669279263

**Email**: preciousvincentct@gmail.com


- - - 
- - - 

# MASTER OSINT advance V4, V5, V6 with new modules are out. 

**kindly check them out via the link below**: 

**https://github.com/techenthusiast167/MASTER-OSINTv4-/blob/main/README.md**

