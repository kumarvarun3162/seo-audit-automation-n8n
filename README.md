# 🚀 SEO Audit Automation with n8n + AI

This project is an automated SEO audit workflow built in [n8n](https://n8n.io).  
It fetches webpages, extracts SEO data, runs AI-powered analysis, and sends structured reports via email.  

---

## ⚙️ Workflow Overview
- **Trigger**: Google Sheets entry (new URL added).
- **Step 1**: Fetch search results via SerpApi.
- **Step 2**: Scrape webpage HTML.
- **Step 3**: Extract title, meta description, H1, H2, paragraphs.
- **Step 4**: AI (Google Gemini) analyzes SEO & generates JSON report.
- **Step 5**: Clean JSON & validate.
- **Step 6**: Send SEO report via Gmail.

---

## 🛠️ Setup
1. Install [n8n](https://docs.n8n.io/getting-started/installation/).
2. Import the workflow JSON:
   - Go to n8n → **Workflows** → **Import from File**.
3. Add your credentials:
   - SerpApi API Key
   - Gmail OAuth
   - Google Sheets integration
   - AI API key (Gemini)
4. Update the `sendTo` email in the Gmail node.

---

## 📩 Example Output
Email report contains:
- SEO Score (/100)
- Major issues found
- Step-by-step improvements

---

## 🚀 Future Improvements
- Bulk URL support
- HTML email reports
- More deterministic SEO checks

---

## 📊 Workflow Diagram

Here’s the visual workflow built in n8n:

![Workflow Screenshot](assets/workflow_screenshot.png)

