# Source-Grounded Business Summaries · ES/PT/EN

**Available on [AWS Marketplace](https://aws.amazon.com/marketplace/pp/prodview-fpr4ku72wwntg), version 0.1.0.** The Public product and Released offer were verified on 14 November 2026. The pinned 0.1.0 model package completed actual AWS validation. The notebook checks the real package status and exact image digest before creating resources. Its code is unexecuted in this repository; saved model responses live in the separate example files below.

Open [sample_notebook.ipynb](sample_notebook.ipynb) for the boto3 real-time, line-split batch and cleanup flow. Subscribe and run in your own SageMaker notebook role session in `us-east-1`. The notebook infers that role and creates a fresh private encrypted evidence bucket. Outside a role session, configure `SAGEMAKER_EXECUTION_ROLE_ARN`; an existing private bucket may be supplied through `SAGEMAKER_DEMO_BUCKET`. Request quota for one `ml.g6e.4xlarge` real-time instance and one optional `ml.g6e.2xlarge` Batch Transform instance. Quota approval does not guarantee AWS capacity.

## Actual recorded examples

- [Real-time input](examples/input.json) → [actual output](examples/output.json), recorded on the exact final image on `ml.g6e.4xlarge`.
- [Batch input](examples/batch-input.jsonl) → [actual EN/ES/PT output](examples/batch-output.jsonl), produced by the completed certification Batch Transform job on `ml.g6e.2xlarge`.

All input text is fictional. Output files are actual AWS responses, not fixtures used to serve inference. The final-image development run admitted 60/60 related AI-authored requests and matched exact action/person/ISO-date metadata in 58/60. These are not independent customer or native-speaker acceptance results. Summary factuality and semantic entailment remain unmeasured. Review every result; exact source quotations identify text, not semantic support.

See the [model card](https://ss-summary-media-637423513289-us-east-1.s3.us-east-1.amazonaws.com/grounded-summary/0.1.0/model-card.html), [evaluation](https://ss-summary-media-637423513289-us-east-1.s3.us-east-1.amazonaws.com/grounded-summary/0.1.0/evaluation.html) and [release status](https://ss-summary-media-637423513289-us-east-1.s3.us-east-1.amazonaws.com/grounded-summary/0.1.0/status.html).

AWS GPU, storage and transfer charges are separate from software charges and any software trial. A measured cold deployment took about 21 minutes; the notebook allows up to 40 minutes for startup. Closing a notebook does not stop an endpoint. Use its cleanup cells and verify removal after failures. Private evidence objects are retained and storage remains billable.

This repository contains public client examples, with no service implementation, weights, private evaluation corpus, credentials or customer documents. GitHub Actions is disabled and no CI/CD is configured. Client examples are licensed under Apache-2.0.

## Video walkthrough

[Watch the English walkthrough](https://www.youtube.com/watch?v=4rDakOYsir4) or the [vertical Short](https://www.youtube.com/shorts/y3dSfPLeQF4). The illustrative UI replays unchanged actual certification outputs for fictional EN/ES/PT inputs; it does not start a new inference job. The UI is not included in the subscription. Narration is AI-generated with NVIDIA Magpie on Jetson AGX Thor. Every draft requires human review.

Software is USD 0.50 per selected instance-hour with a 14-day software trial; AWS infrastructure remains separately billable throughout. Follow the [buyer guide](https://ss-summary-media-637423513289-us-east-1.s3.us-east-1.amazonaws.com/grounded-summary/0.1.0/usage.html) for limits, supported instances and cleanup.
