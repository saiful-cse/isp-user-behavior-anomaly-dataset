# Anonymized ISP Event-Level Traffic Dataset for User Behavior Analysis

This repository contains an anonymized ISP network traffic dataset used for user behavior analysis and unsupervised anomaly detection. The data are derived from real operational ISP logs and are provided at the event level with anonymized user identifiers. The dataset has been processed to ensure privacy preservation and ethical compliance and is intended strictly for academic and research purposes.

---

## Dataset Description

The dataset consists of network traffic metadata collected during routine ISP monitoring operations. Each record represents an individual network traffic event associated with an anonymized user identifier, without exposing any personally identifiable information or organizational identifiers. User-level behavior profiles used in the associated study are derived by aggregating these event-level records prior to analysis.

The data are suitable for studies on:
- User behavior analysis  
- Unsupervised anomaly detection  
- Network traffic characterization  
- Privacy-preserving network analytics  

### 📥 Data Access
The complete anonymized dataset (`user_logs_anonymized_546278_row.csv`) is publicly available and can be downloaded from the following secure repository:
👉 **[Download Dataset via Google Drive][https://drive.google.com/file/d/1kiHEJ6hzMuoa48y3BS45Y1-N1-T_SkX9/view?usp=sharing]**

---

## Anonymization and Privacy Protection

To ensure privacy and confidentiality, the following anonymization steps have been applied:

- User identifiers are irreversibly hashed and encoded into numeric user IDs.
- Source and destination IP addresses have been completely removed.
- No packet payload or application-level content is included.
- No ISP name, geographic identifier, or organizational metadata is disclosed.
- Logged timestamps are left completely unaltered. Since the associated framework relies purely on aggregated statistical metadata rather than sequential time-series tracking, explicit temporal sequence processing was omitted.

As a result, the dataset does not allow re-identification of users or the originating ISP.

---

## Dataset Structure

The anonymized dataset is provided in CSV format with the following fields:

| Column Name | Description |
|------------|-------------|
| `timestamp` | Time of the traffic event (Original unaltered format) |
| `user_id` | Encoded numeric user identifier |
| `protocol` | Network protocol (e.g., TCP, UDP) |
| `src_port` | Source port number |
| `dst_port` | Destination port number |
| `length` | Packet length in bytes |

All features are metadata-level attributes only.

---

## Intended Use

This dataset is intended for:
- Offline research and experimentation
- Development and evaluation of unsupervised learning methods
- Event-level analysis and user-level aggregation for behavioral modeling

The dataset is **not** intended for:
- Real-time intrusion detection deployment
- Commercial use
- User profiling or surveillance
- Policy enforcement or traffic blocking

---

## Reproducibility & Source Code

To ensure full transparency and reproducibility of the published results, the complete source code configurations, including the raw data anonymization pipeline logic and machine learning models, are provided in this repository.

- You can view and run the replication notebook directly here: **[Google Colab / Jupyter Notebook Link]([https://colab.research.google.com/drive/1VFniaTWKr1Dq3eH3p6nBn9PfhrS2p6jq?usp=sharing])**

Researchers are encouraged to cite the associated publication when using this dataset or code in academic work.

---

## Ethical Considerations

The dataset has been anonymized following standard ethical practices for handling network traffic data. No consent-sensitive information, payload data, or identifying metadata is included. The dataset is shared solely to advance research in privacy-preserving network security and behavior analysis.

---

## License

This dataset is released for **research and academic use only**.  
Users are responsible for ensuring compliance with applicable data protection and ethical guidelines when using the dataset.

---

## Citation

If you use this dataset in your research, please cite the associated article:

> *AI-Driven User Behavior Analysis and Anomaly Detection in ISP Networks*,  
> Journal (ongoing...)

(Full citation details will be added upon publication.)
