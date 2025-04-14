Introduction A smart grid integrates intelligent sensors and meters, connecting to central servers or cloud platforms via wired or wireless networks. It improves energy management through methods such as framework analysis and dynamic load scheduling, reducing peak usage and enhancing cost-efficiency. Smart grids support sustainable development by combining power system architecture with digital technology to monitor customer behavior and forecast energy use. This integration forms the Energy Internet (EI), where the Advanced Metering Infrastructure (AMI) provides utilities with detailed energy usage data for forecasting and demand response. Non-technical losses (NTL), such as power theft and irregular billing, cause significant economic losses. Smart meter-based solutions detect NTL by analyzing consumption patterns and identifying anomalies. However, high deployment costs and cybersecurity risks present challenges. AI and deep learning techniques help detect energy theft by analyzing user consumption patterns. Compared to hardware-based methods, AI and game theory-based approaches are more cost-effective and efficient. Game theory models interactions between providers and fraudulent users, while machine learning identifies abnormal usage behaviors. The study explores federated learning (FL)-based deep learning methods for electricity theft detection, focusing on data privacy while analyzing consumer behavior. It introduces a hybrid FL-based model, offering a novel approach to theft detection.

**DATASET USED**: https://data.mendeley.com/datasets/c3c7329tjj/3

A suitable dataset consisting of 58,565 samples from which 20000 samples were used for analysis . This dataset is designed for benchmarking and machine learning-based classification in smart grid environments . It includes various types of simulated theft scenarios, making it valuable for analyzing consumption patterns and detecting irregular usage.

**Anomalies Predicted**

**Anomalies in Electricity Consumption**
Highlighted Anomalies: 
• Red dots mark anomalous points, clearly identifying deviations from normal behavior. 
• These points correspond to hours with unusual spikes or drops in consumption.
Temporal Patterns: 
• Anomalies are isolated events, suggesting they may be caused by external factors (e.g., tampering, sudden load changes). 
Applications 
• Electricity Theft Detection: 
• Spikes (e.g., hour 200) may indicate unauthorized tapping into the grid. 
• Drops (e.g., hour 800) could result from meter bypassing or tampering.

**Anomalies in Normal consumption**
In this Plot the high value of 200 kWh at 5:00 is not flagged as an anomaly because it might fall within the acceptable range of variability for normal consumption patterns. This could happen due to the following reasons:

**Threshold-Based Anomaly Detection** 
• The anomaly detection algorithm likely uses a predefined threshold (e.g., ±2 standard deviations from the mean or a specific percentile). If the value of 200 kWh is below this threshold, it will not be flagged as an anomaly. 
• For example: 
  • Mean consumption = 100 kWh 
  • Standard deviation = 50 kWh 
  • Threshold = Mean + 2 × SD = 200 kWh 
  • Since the spike equals the threshold, it may not be flagged.

**Contextual Variability** 
• The algorithm may account for time-of-day patterns. High consumption during certain hours (e.g., early morning or peak hours) might be common in some scenarios, so the spike at 5:00 could be considered normal.
