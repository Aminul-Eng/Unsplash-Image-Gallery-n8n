# Dynamic Unsplash Image Gallery via n8n 📸✨

An automated workflow built with **n8n** that accepts query parameters via a Webhook, fetches high-quality images from the **Unsplash REST API** using proper authentication, processes the JSON response, and renders a dynamic image gallery directly in the browser.

## 🚀 Project Overview
This project demonstrates how to connect third-party APIs inside n8n, handle API authentication using Access Keys, process complex JSON payloads, and respond dynamically to web requests.

## ✨ Features & What I Learned
- **API Integration & Auth:** Created an application in Unsplash Developer Portal and utilized API Keys (Access Keys) for secure authentication.
- **Webhook Trigger:** Configured an n8n Webhook to accept dynamic URL Query Parameters (e.g., `?q=coffee`).
- **REST API Request:** Used HTTP Request nodes to communicate with Unsplash REST endpoints.
- **Data Processing:** Processed and extracted essential data (Image URLs and Descriptions) from the JSON response using Edit Fields nodes.
- **Dynamic Response Rendering:** Used the Respond to Webhook node to present a fully formatted, dynamic image gallery directly in the browser.

---

## 🛠️ Tech Stack
* **n8n:** Low-code automation and workflow orchestration.
* **Unsplash API:** For fetching real-time image data and assets.
* **Webhooks & REST APIs:** For triggering and handling HTTP requests/responses.

---

## 🔑 How to Configure Unsplash API
1. Log in to your [Unsplash Developer Portal](https://unsplash.com/developers).
2. Register a new application and grab your **Access Key**.
3. In n8n, use an HTTP Request node with Header Authentication (`Client-ID YOUR_ACCESS_KEY`).

---

## 🖼️ Workflow & Output Screenshots
### 1. n8n Workflow Architecture
![Workflow Architecture](./workflow.png)

---

## 🚀 How to Use
1. Download the `workflow.json` file from this repository.
2. Import it into your n8n workspace.
3. Configure your Unsplash API Access Key credentials.
4. Activate the webhook URL and test it in your browser with a query parameter (e.g., `your-webhook-url?q=nature`).
