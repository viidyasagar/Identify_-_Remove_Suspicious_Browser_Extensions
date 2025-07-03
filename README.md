## 📌 Objective

The objective of this task is to **identify and remove suspicious or unnecessary browser extensions** in Kali Linux, focusing on Firefox (default browser), in order to enhance security and browser performance. Additionally, this task serves to document awareness of how malicious extensions operate and their potential impacts on user systems.

---

## 🖥️ Environment

* **Operating System**: Kali Linux (Rolling Edition)
* **Browser Used**: Mozilla Firefox (Default in Kali)
* **User Privileges**: Non-root user with GUI access
* **Tools**: Built-in Firefox Add-ons Manager

---

## 📋 Task Description

A detailed walkthrough of performing a **manual extension audit** in Firefox on Kali Linux.

### 1️⃣ Open Extension/Add-ons Manager

* Launch **Firefox** from the Applications menu or terminal.
* Click the **hamburger menu (☰)** on the top-right corner.
* Navigate to **"Add-ons and Themes"** or press `Ctrl + Shift + A` to access the Add-ons Manager.
* Choose the **Extensions** tab.

---

### 2️⃣ Review All Installed Extensions

* Carefully inspect the list of installed extensions.
* Identify each extension by name, publisher, and icon.
* Note extensions that were not explicitly installed by the user or look unfamiliar.

---

### 3️⃣ Check Permissions and User Reviews

* For each extension:

  * Click on the **three-dot menu** → **"Manage"**.
  * Review the permissions it requires (e.g., access to all websites, clipboard, tabs).
  * Click **"More Information"** to open the extension's page on Mozilla’s Add-ons website.
  * Check the number of downloads, user reviews, last update date, and developer credibility.

---

### 4️⃣ Identify Suspicious or Unused Extensions

Red flags for suspicious extensions may include:

* Excessive or unnecessary permissions (e.g., access to all browsing data).
* Poor or no user reviews.
* Outdated or rarely updated extensions.
* Unknown or unverifiable publishers.
* Abnormal behavior observed during browsing.

---

### 5️⃣ Remove Unwanted Extensions

* For each identified extension:

  * Click the **three-dot menu** → select **"Remove"**.
  * Confirm removal when prompted.

---

### 6️⃣ Restart Firefox

* Fully close the Firefox browser.
* Reopen it and check:

  * If browser performance has improved (load times, responsiveness).
  * If any previous redirections or pop-ups are no longer appearing.

---

### 7️⃣ Research on Malicious Extension Behaviors

Malicious browser extensions can pose significant security and privacy risks. Some known risks include:

| Threat               | Description                                               |
| -------------------- | --------------------------------------------------------- |
| **Credential Theft** | Capture login details entered into forms.                 |
| **Ad Injection**     | Display unauthorized ads or pop-ups.                      |
| **Tracking**         | Monitor browsing behavior and send data to third parties. |
| **Clickjacking**     | Interfere with browser interaction or mask content.       |
| **Redirection**      | Redirect users to phishing or malicious websites.         |

Resources used:

* [Malwarebytes Blog](https://www.malwarebytes.com/blog)
* [Mozilla Extension Policies](https://extensionworkshop.com/documentation/publish/add-on-policies/)

---

### 8️⃣ Documentation of Actions Taken

A log file was created to maintain records of extensions removed and actions taken.

#### Example Log File:

```bash
# File: extension_cleanup_log.txt
Date: 2025-07-03

Removed Extension: "Dark PDF Converter"
Reason: Unknown publisher, requested clipboard and tab access
Action: Removed via Firefox Manager, browser restarted, no issues observed.

Removed Extension: "SuperSearch Enhancer"
Reason: Suspicious permissions and poor reviews
Action: Removed, confirmed performance improvement.
```

To create the log:

```bash
nano extension_cleanup_log.txt
```

Use `Ctrl + O`, `Enter`, then `Ctrl + X` to save and exit.

---

## ✅ Outcome

* Unnecessary and suspicious extensions successfully removed.
* Browser performance improved with faster load time and reduced lag.
* Better understanding of extension permissions and potential security threats.
* Clean documentation and audit log maintained.

---

## 📎 Future Recommendations

* Perform regular audits of browser extensions.
* Avoid installing extensions from unknown or unverified developers.
* Keep browsers and extensions up to date.
* Use sandbox environments to test new extensions before deploying on production systems.

---

