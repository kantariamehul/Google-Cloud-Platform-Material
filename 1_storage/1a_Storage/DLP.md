# Storage Tools

## DLP Scanning (Data Loss Prevention)
Fully managed service designed to help you discover, classify, and protect your most sensitive data.
- list of types of PII identified - [link](https://cloud.google.com/dlp/docs/infotypes-reference?hl=en_US)
- de-identify PII data with DLP - [link](https://cloud.google.com/architecture/de-identification-re-identification-pii-using-cloud-dlp)
- use cases for DLP -[link](https://cloud.google.com/dlp#section-6) - and shown in Google's diagram below

<img src="https://www.gstatic.com/bricks/image/17ce743c5356e76389a971b4267faca0331ad0c6dd28a0eb6728565c23cb9704.svg">

## ClamVar Virus Scanning
Automating malware scanning for documents uploaded to Cloud Storage - [link](https://cloud.google.com/architecture/automating-malware-scanning-for-documents-uploaded-to-cloud-storage)
  - Build using GCP with an open source antivirus engine called ClamAV
  - Run ClamAV in a Docker container hosted in Cloud Run (architecture shown below)
  - Write log entries to Cloud Logging and records metrics to Cloud Monitoring
  - Builds an event-driven pipeline that can help you automate the evaluation of documents for malicious code

<img src="https://github.com/lynnlangit/gcp-essentials/blob/master/1_storage/1a_Storage/images/clamvar-cloudrun.png" width=800>
  
   
