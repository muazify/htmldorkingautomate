# Advanced Site Dorking Tool

A browser-based HTML/JavaScript tool to automate Google Dorking against a specific target domain using a comprehensive set of predefined search templates.

**Repository:** [https://github.com/muazify/htmldorkingautomate](https://github.com/muazify/htmldorkingautomate)

## 📜 Description

This tool provides a simple web interface to generate and execute numerous Google Dork queries tailored for security reconnaissance. By providing a target domain and optional parameters like keywords, excluded filetypes, and specific paths, users can quickly launch advanced searches designed to uncover potential misconfigurations, sensitive information exposure, vulnerable components, and more. The tool runs entirely client-side, leveraging JavaScript to construct and open search queries in new browser tabs.

## ✨ Features

* **Target Domain Specificity:** Focuses all dorks on a single `site:` operator.
* **Keyword/Phrase Integration:** Incorporates user-defined keywords and quoted phrases into dorks.
* **Filetype Exclusion:** Filters results by excluding specified file extensions (`-filetype:`).
* **Path Targeting:** Narrows searches to specific URL paths (`inurl:` or combined with `site:`).
* **Extensive Dork Template Library:** Includes dozens of pre-configured dorks covering:
    * Configuration Files (env, cfg, ini, xml, yml, etc.)
    * Log Files
    * Admin/Login Interfaces
    * Sensitive Keywords (password, api_key, secret, etc.)
    * Directory Listings
    * Subdomain Discovery
    * Backup Files & Directories (sql, bak, zip, dump)
    * Cloud Keys & Secrets (AWS, Private Keys)
    * Technology Footprints (PHPInfo, WP, Magento, Nginx, Tomcat, Struts)
    * Common Vulnerable Parameter Patterns
* **Client-Side Execution:** Runs entirely in the browser. No installation or backend needed.
* **Automated Tab Opening:** Attempts to open each generated Google Search URL in a new browser tab.
* **Pop-Up Blocker Awareness:** Provides feedback if pop-ups seem blocked.
* **Duplicate Query Prevention:** Avoids launching identical searches.
* **Basic Input Validation:** Checks domain format.
* **Clean Interface:** Simple Bootstrap 5 based UI.

## 🚀 How to Use

1.  **Get the Code:**
    * Clone the repository: `git clone https://github.com/muazify/htmldorkingautomate.git`
    * OR Download the ZIP file from the repository page and extract it.
2.  **Open the Tool:**
    * Navigate to the extracted directory.
    * Open the main HTML file `Dorking_mate.html`in your preferred web browser (Firefox, Chrome, Edge, etc.).
3.  **❗️ Enable Pop-ups ❗️:**
    * This tool **REQUIRES** pop-ups to be enabled for the page to function.
    * When you first try to run dorks, your browser will likely block the pop-ups. Look for an icon or message in the address bar or elsewhere in the browser UI.
    * Click the icon/message and choose **"Always allow pop-ups and redirects from [file path/origin]"**. You may need to click the "Run Advanced Dorks" button again after enabling pop-ups.
4.  **Fill the Form:**
    * **Target Site/Domain (Required):** Enter the domain you want to search (e.g., `example.com`, `sub.example.co.uk`). Do *not* include `http://` or `https://`.
    * **Keywords/Phrases (Optional):** Enter space-separated keywords. Use quotes for exact phrases (e.g., `database backup "api key" confidential`).
    * **Exclude File Extensions (Optional):** Enter comma-separated file extensions *without the dot* (e.g., `html, css, js, png, jpg`).
    * **Specific Path (Optional):** Enter a path to focus on (e.g., `/admin`, `/uploads`, `/files/private`). A leading slash `/` will be added if missing.
5.  **Run Dorks:**
    * Click the "Run Advanced Dorks" button.
6.  **Review Results:**
    * The tool will generate dork queries based on the inputs and its internal templates.
    * It will then attempt to open each unique, valid query in a new browser tab using Google Search.
    * Check the feedback message in the tool for the number of dorks attempted/opened and any pop-up warnings.
    * Analyze the results in the newly opened tabs.

## 🖼️ Screenshot
![image](https://github.com/user-attachments/assets/864b325f-6917-4ea4-91f4-4b2b927fa335)

## ⚠️ Disclaimer
This tool is provided for educational and legitimate security research purposes only. DO NOT use this tool to conduct unauthorized scanning or searching against systems you do not have explicit permission to test. Misuse of Google Dorking techniques can lead to unintentional access to sensitive information and may be illegal in your jurisdiction. The user assumes all responsibility for their actions when using this tool. Always act ethically and legally.

## 🤝 Contributing
Contributions are welcome! If you have ideas for new dork templates, improvements to the JavaScript logic, or UI enhancements, feel free to:

* Fork the repository.
* Create a new branch (`git checkout -b feature/YourFeature`).
* Make your changes.
* Commit your changes (`git commit -m 'Add some feature'`).
* Push to the branch (`git push origin feature/YourFeature`).
* Open a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
