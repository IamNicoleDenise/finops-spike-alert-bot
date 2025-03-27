
# 🧠 FinOps Spike Alert Bot

A lightweight, automated solution for detecting AWS cost anomalies and sending real-time Slack alerts.

Built for busy teams and solo builders who want to monitor spend spikes without constantly checking Cost Explorer.

## 🚀 What It Does

- ✅ Analyzes daily AWS cost data (CSV-based)  
- ✅ Detects spend spikes using a 7-day average vs. yesterday  
- ✅ Sends Slack alerts when thresholds are breached  
- ✅ (Optional) Generates a bar chart of cost comparisons  
![cost_comparison_chart](https://github.com/user-attachments/assets/1bf8c712-09c0-49b4-bd7b-a372eb097c8b)

## 📁 Project Structure

```
FinOpsSpikeAlertBot/
├── .env                        # Stores your Slack Bot Token (excluded from Git)
├── finops_spike_alert.ipynb    # Main notebook to run and test the bot
├── dummy_aws_cost_data.csv     # Sample AWS cost data for testing
├── cost_comparison_chart.png   # (Optional) chart image output
├── README.md                   # You're reading it
```

## 🛠️ Setup Instructions

1. **Clone or download** this repo  
2. Create a `.env` file in the root folder and add: Your Slack Token
3. Open `finops_spike_alert.ipynb` and run it step by step  
4. Your Slack bot will send an alert if a cost spike is detected

## 📌 Notes

- Uses Slack **bot tokens**, not incoming webhooks  
- Slack image uploads are optional — use hosted links if needed  
- Cost data comes from a CUR or Cost Explorer export (CSV)  

## 💡 Future Enhancements

- Auto-upload chart to S3 + share link  
- GitHub Actions or AWS Lambda for daily runs  
- Multi-account AWS cost aggregation  
- Enhanced anomaly detection (z-score, rolling windows)  

## 👩🏽‍💻 Created By

**Nicole Coleman**  
Freelancer @ 3509 Innovation  
AWS Community Builder • FinOps + Automation Specialist


