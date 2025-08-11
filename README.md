# Pipedrive-to-Slack Automated Activity Alerts

**Client Industry:** B2B Sales & CRM Management  
**Tools Used:** n8n, Pipedrive API, Slack API, JavaScript (Custom Code Node)

---

## 📌 Problem

The client’s sales team was frequently missing critical follow-ups because Pipedrive activity notifications were either delayed or buried in email inboxes.

**Key Issues:**
- Missed due dates for high-value deals.
- Manual checking of Pipedrive multiple times a day.
- No central channel for tracking updates across the team.

---

## 💡 Solution

I designed and implemented an **automated workflow** using **n8n** to instantly send formatted activity notifications from Pipedrive to Slack.

**Key Features:**
1. **Real-time Webhook Trigger** – Captures any new or updated activities in Pipedrive.
2. **Dynamic Data Retrieval** – Fetches complete activity details (subject, assigned user, due date/time, type, note) and associated deal info (deal title, contact details, stage).
3. **Custom Code Formatting** – Uses JavaScript in n8n’s Code node to clean, structure, and map CRM data into a Slack-friendly format.
4. **Direct Slack Delivery** – Posts alerts into a designated Slack sales channel with clickable links to the relevant Pipedrive deal.

---

## 📈 Impact

- **Zero missed follow-ups** – the team now acts on updates immediately.
- **Single source of truth** for all sales activity in Slack.
- **Saved 2+ hours daily** previously spent checking Pipedrive manually.

---

## 🖼️ Workflow Diagram

*(Optional – add an image or screenshot of your n8n workflow here)*

---

## 🚀 How It Works

1. **Trigger:** Pipedrive Webhook → `n8n Webhook Node`
2. **Data Fetch:** `HTTP Request Node` to Pipedrive API for activity and deal details
3. **Data Processing:** `Code Node (JavaScript)` for formatting
4. **Delivery:** `Slack Node` to post the alert

---

## 🔗 Related Links
- [n8n Documentation](https://docs.n8n.io/)
- [Pipedrive API Docs](https://developers.pipedrive.com/docs/api/v1/)
- [Slack API Docs](https://api.slack.com/)

