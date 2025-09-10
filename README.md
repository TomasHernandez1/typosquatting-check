# typosquatting-check
typosquatting-check analyzes domains using dnstwist, checks if they are active, and integrates with VirusTotal to detect malicious ones.

# Features
- Generates domain permutations via dnstwist
- Detects if a domain is registered/active
- Scans domains with VirusTotal API v3
- Saves results into Excel reports

# Usage
1. Prepare an Excel file (.xlsx) with a column named 'domain', for example:

example.com

test.com

domain.org

2. Run the script and pass the file as an argument:
```bash
python3 typos.py <domains.xlsx>
```

# Output example
```console
$ python script.py -i domains.xlsx
Processing dnstwist for domain: example.com...
dnstwist processing completed
Starting Virustotal scan...
Virustotal scan completed
The file risultati/example.com.xlsx is ready
```
