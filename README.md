# Arachnid

Arachnid is a powerful and efficient web crawler built using Python's `asyncio` library for asynchronous operations. It's designed to explore websites thoroughly, gathering valuable information and providing insightful reports.

## Features

- **Asynchronous Crawling:** Leverages `asyncio` for fast and efficient crawling of multiple pages concurrently.
- **Subdomain Discovery:**  Discovers subdomains using a combination of techniques:
    - DNS Zone Transfers
    - Brute-force enumeration (using a customizable wordlist)
    - Scraping search engine results
- **Dynamic Rendering:** Optionally uses Playwright to render JavaScript-heavy websites and extract content accurately.
- **Robots.txt Adherence:** Respects `robots.txt` rules to ensure ethical crawling practices.
- **Robust Error Handling:** Handles various exceptions gracefully to prevent interruptions during crawling.
- **Rich TUI:** Provides a visually appealing terminal interface using the `rich` library, including:
    - ASCII art title
    - Progress bars
    - Formatted tables
    - Informative panels
- **Detailed Reports:** Generates comprehensive reports in JSON and Excel formats, including:
    - Crawling summary (pages crawled, failed URLs)
    - Performance metrics (average load time)
    - Status code distribution
    - Content type distribution
    - List of visited pages with metadata (URL, title, status code)

## Installation

1. **Create a virtual machine (optional, but recommended)**
  ```bash
  python -m venv venv
  source venv/bin/activate for windows venv\bin\activate
  ```


3. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/arachnid.git
   cd arachnid
   pip install -r requirements.txt
   python Arachnid.py
   ```

## Usage

1. **Provide a wordlist for subdomain enumeration (optional):**

- Create a file named subdomains.txt (or customize the filename in the code).

- Add common subdomain names to this file, one per line.

**Run the crawler:**
```bash
python arachnid.py
```
3. Enter the target website URL when prompted.

4. Arachnid will start crawling the website and display progress in the terminal.

5. Upon completion, reports will be generated in the following formats:

- ```crawler_report.json```

- ```crawler_report.xlsx```

## Tested Operating Systems

<table>
    <tr>
        <th>Operative system</th>
        <th> Version </th>
    </tr>
    <tr>
        <td>Windows</td>
        <td>11/10</td>
    <tr>
        <td>MacOS</td>
        <td>10.15+</td>
    </tr>
    <tr>
        <td>Linux (Ubuntu)</td>
        <td>20.04+</td>
    </tr>
    
  
</table>
Anything below the specified OS version is not guaranteed to work and it's not going to be fixed/added

## ● Contribution Guidelines
Contributions are welcome! If you’re interested in helping improve ExeialRR, please consider the following:
- Check the issues tab for current tasks.
- Fork the repository and create a pull request.
- Share your feedback and suggestions.
 
Your support is greatly appreciated, as I am a solo developer and still learning. Thank you!
If you want to contact me, dm @mylifeislag by discord.

