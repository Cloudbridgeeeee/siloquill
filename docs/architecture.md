# Proposed AWS architecture

| Service | Role |
|---|---|
| S3 and Lambda | Stock records and scans, checked as they arrive |
| Textract | Waybills and delivery notes read into rows |
| SageMaker AI | Storage demand and capacity models per store |
| DynamoDB | Stores, batches, counts and the decision log |

One AWS account per customer, encrypted at rest and in transit. The public demo calls none of these services.
