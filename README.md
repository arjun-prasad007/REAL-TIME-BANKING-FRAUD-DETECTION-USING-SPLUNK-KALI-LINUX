🛡 Real-Time Banking Fraud Detection System
Splunk + Kali Linux Simulation
📝 Project Overview
Ithu banking transactions-il nadakkunna "Impossible Travel" fraud detect cheyyaanulla oru SIEM project aanu. Kali Linux upayogichu fraudulent transactions inject cheyyunnathum, athu Splunk vazhi real-time aayi detect cheythu dashboard create cheyyunnathum aanu ee project-inte main objective.
🛠 Tools Used
SIEM: Splunk Enterprise (v10.2.0)
Attacker Machine: Kali Linux (Simulation)
Data Source: CSV-based Banking Transactions
🚀 Simulation Steps
Attack Injection: Kali Linux terminal vazhi Sharjah-yil ninnulla fraud transaction entries banking_transactions.csv file-ilekku inject cheythu.
Log Monitoring: Splunk aa file-ile changes real-time aayi monitor cheythu 8-il adhikam Sharjah transactions detect cheythu.
Fraud Detection Logic: Thazhe ulla SPL (Splunk Processing Language) upayogichu ore Account ID-il ninnu different cities-il (Dubai, Abu Dhabi, Sharjah) nadanna transactions thirichariju.
🔍 SPL Query Used:

source="banking_transactions.csv" 
| stats dc(Location) as city_count, values(Location) as Cities by Account_ID 
| where city_count > 1

![](/assets/STATISTICS.png)
![](/assets/GRAPH.png)
![](/assets/KALI.png)
![](/assets/ATTACK.png)
![](/assets/ID.png)
