# Automated Technical Sales Lead Pipeline (Tally + Make + Salesforce)

An enterprise-grade lead ingestion system built to automate lead capture, eliminate manual data entry, and instantly map inbound prospects into Salesforce Sales Cloud for immediate sales outreach.

---

## 🎯 Business Impact
* **Zero Manual Entry:** Automated lead ingestion directly from web forms into Salesforce CRM.
* **Instant Speed-to-Lead:** Sub-second delivery of web submissions to the sales team via real-time webhooks.
* **Data Integrity:** Enforced standard schema mapping for core Lead attributes (Last Name, Company, Email, Phone).
* **Target Scale:** Engineered to support sales operations aiming for $200,000+ ARR pipelines.

---

## 🛠️ Architecture & Tech Stack

```text
[Tally.so Form Submission] 
            │
            ▼ (HTTPS POST Webhook)
  [Make.com Middleware Engine] 
            │
            ▼ (OAuth 2.0 REST API)
  [Salesforce Sales Cloud] ───> (Lead Record Created)
```
* **Lead Capture:** Tally.so (Custom Webhook Integration)
* **Automation Orchestration:** Make.com (OAuth 2.0 / REST)
* **CRM Platform:** Salesforce Cloud (Standard Lead Object)

---

## 📦 Blueprint Deployment
To deploy this scenario in your own Make.com organization:
1. Download the `blueprint.json` file from this repository.
2. In Make.com, create a new scenario and select **Import Blueprint** from the options menu.
3. Re-authorize your Salesforce connection via Interactive OAuth2.
4. Copy your Make webhook URL into your Tally form integration settings.
