<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/control-plane-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/control-plane-light.svg">
  <img alt="Sujaya Mindev - software engineer building applications and the infrastructure beneath them" src="./assets/control-plane-light.svg" width="100%">
</picture>

<br>

[sujaya.dev](https://sujaya.dev) &nbsp;&middot;&nbsp; [LinkedIn](https://www.linkedin.com/in/sujayamindev) &nbsp;&middot;&nbsp; [Repositories](https://github.com/sujayamindev?tab=repositories)

</div>

## 01 / OPERATING RANGE

I'm **Sujaya Mindev**, a Computer Science (Software Engineering) undergraduate building across the boundary between product software and cloud infrastructure.

I like systems where every layer has to work together: the interface people touch, the APIs behind it, the data moving through it, and the delivery pipeline that keeps the whole thing running.

## 02 / DEPLOYED SYSTEMS

### 001 &mdash; [Reclaima](https://github.com/sujayamindev/reclaima)

**Turn a fading receipt into a claim-ready record.** Reclaima is an offline-first mobile app that extracts receipt data, tracks per-item warranties and return windows, sends deadline reminders, and generates claim PDFs.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/reclaima-system-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/reclaima-system-light.svg">
  <img alt="Reclaima system architecture: Flutter and SQLite through KrakenD and FastAPI to PostgreSQL, with AWS Textract and Bedrock OCR processing" src="./assets/reclaima-system-light.svg" width="100%">
</picture>

- Offline-first Flutter client backed by Drift and SQLite.
- FastAPI and PostgreSQL behind a KrakenD gateway with JWT validation and rate limiting.
- OCR through AWS Textract with a Claude Haiku cleanup layer; deployed with Docker and Terraform on OCI, with CI/CD and observability.

[Explore the case study &rarr;](https://sujaya.dev/reclaima) &nbsp;&nbsp; [View the source &rarr;](https://github.com/sujayamindev/reclaima)

---

### 002 &mdash; [Serverless Media Upload Pipeline](https://github.com/sujayamindev/serverless-media-upload-pipeline)

**A zero-trust upload path where the API stays out of the file transfer.** The browser uploads directly to S3 using a presigned POST; an event-driven validation path decides what can be delivered.

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/media-pipeline-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="./assets/media-pipeline-light.svg">
  <img alt="Serverless media upload architecture: browser requests a presigned upload, sends the file to S3, and an ObjectCreated event triggers Lambda validation with DynamoDB status and CloudFront delivery" src="./assets/media-pipeline-light.svg" width="100%">
</picture>

- Direct-to-S3 uploads using presigned POSTs instead of proxying files through the API.
- Binary content validation on <code>ObjectCreated</code>, with approve/reject state tracked in DynamoDB.
- Cognito authentication, CloudFront delivery, Terraform infrastructure, and a tested GitHub Actions pipeline.

[Explore the case study &rarr;](https://sujaya.dev/serverless-pipeline) &nbsp;&nbsp; [View the source &rarr;](https://github.com/sujayamindev/serverless-media-upload-pipeline)

## 03 / BUILD LAYERS

| Layer | Working with |
|:--|:--|
| **Interfaces** | Flutter &middot; React &middot; Next.js |
| **Services** | FastAPI &middot; Node.js &middot; Spring &middot; REST APIs |
| **Data** | PostgreSQL &middot; SQLite &middot; DynamoDB |
| **Cloud** | AWS &middot; OCI &middot; Docker &middot; Terraform |
| **Delivery** | GitHub Actions &middot; CI/CD &middot; Observability |

---

<div align="center">

**APPLICATIONS / INFRASTRUCTURE / DELIVERY**

<sub>Build the product. Understand the system. Own the path to production.</sub>

</div>
