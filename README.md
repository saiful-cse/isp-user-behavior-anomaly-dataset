# Anonymized ISP User-Level Traffic Dataset

This repository contains an anonymized ISP network traffic dataset used for user-level behavior analysis and unsupervised anomaly detection. The data are derived from real operational ISP logs and have been processed to ensure privacy preservation and ethical compliance. The dataset is intended strictly for academic and research purposes.

---

## Dataset Description

The dataset consists of network traffic metadata collected during routine ISP monitoring operations. Each record represents a network traffic event associated with a user, without exposing any personally identifiable information or organizational identifiers. The dataset is designed to support offline analysis of user behavior through aggregated traffic characteristics.

The data are suitable for studies on:
- User behavior analysis  
- Unsupervised anomaly detection  
- Network traffic characterization  
- Privacy-preserving network analytics  

---

## Anonymization and Privacy Protection

To ensure privacy and confidentiality, the following anonymization steps have been applied:

- User identifiers are irreversibly hashed and encoded into numeric user IDs.
- Source and destination IP addresses have been removed.
- No packet payload or application-level content is included.
- No ISP name, geographic identifier, or organizational metadata is disclosed.
- Timestamp information is retained only for temporal analysis and does not enable user identification.

As a result, the dataset does not allow re-identification of users or the originating ISP.

---

## Dataset Structure

The anonymized dataset is provided in CSV format with the following fields:

| Column Name | Description |
|------------|-------------|
| `timestamp` | Time of the traffic event (coarse-grained) |
| `user_id` | Encoded user identifier |
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
- User-level aggregation and behavioral modeling

The dataset is **not** intended for:
- Real-time intrusion detection deployment
- Commercial use
- User profiling or surveillance
- Policy enforcement or traffic blocking

---

## Reproducibility

The dataset supports reproducibility of published research by providing:
- Fully anonymized raw event-level traffic logs
- Consistent feature definitions
- User-level aggregation compatibility

Researchers are encouraged to cite the associated publication when using this dataset in academic work.

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
> Journal of Network and Computer Applications (Elsevier).

(Full citation details will be added upon publication.)

---
