# Origin Finder 🔍🚀

Identify the origin IP address of a domain behind a CDN by leveraging subdomain enumeration, DNS lookups, and Shodan historical data.

## ⚡️ Features

* Subdomain Enumeration using crt.sh
* DNS Lookup for CDN IP addresses
* Shodan Historical IP Search
* Content Matching to Identify Origin IPs
* Detection of Missing CDN Headers

## 🚀 Installation

1. Clone the repository:

```bash
git clone https://github.com/cdrom0/OriginFinder.git
cd OriginFinder
```

2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

3. Obtain Shodan API Key and configure it in `utils/shodan_utils.py`.

## ✅ Usage

Run the script with a target domain:

```bash
python OriginFinder.py <domain>
```

Example:

```bash
python OriginFinder.py example.com
```

## 📦 Output

* Displays CDN IPs, Subdomains, Shodan IPs, and potential origin IPs.
* Identifies missing CDN headers that indicate origin exposure.

## ⚠️ Disclaimer

This tool is intended for educational purposes only. Unauthorized usage against domains without proper authorization is strictly prohibited.

## 🛠️ Contributing

* Fork the repository
* Create a new branch (`git checkout -b feature/your-feature`)
* Commit your changes (`git commit -am 'Add new feature'`)
* Push to the branch (`git push origin feature/your-feature`)
* Open a Pull Request
