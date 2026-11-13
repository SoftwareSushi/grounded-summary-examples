# Source-Grounded Business Summaries · ES/PT/EN

**Unreleased technical preview.** This product is not available for subscription yet. The notebook intentionally stops before any AWS operation until the certified package ARN and image digest are populated from actual release evidence. No output is fabricated or stored in the notebook.

Open [sample_notebook.ipynb](sample_notebook.ipynb) for the prepared boto3 real-time and line-split batch flow, fictional multilingual requests, and compute cleanup. The preview targets `us-east-1` and one `ml.g6e.2xlarge` instance. After release it will require a subscription, permissions in your AWS account, and the corresponding real-time/batch quotas.

`examples/input.json` is a direct invocation body. `examples/batch-input.jsonl` contains one request per line. These inputs are fictional. Actual qualified output samples will be added after the matching AWS image passes its release gates.

Review every generated result. Exact source quotations identify source text; they do not establish semantic support or guarantee factual correctness. Independent bilingual acceptance has not been completed.

AWS GPU, storage and transfer charges are separate from software charges and any software trial. Closing a notebook does not stop an endpoint; use its cleanup cells and verify the resources are removed.

This repository contains only public client examples. It contains no service code, weights, private evaluation corpus, credentials, or customer documents. No CI/CD is configured. Examples are licensed under Apache-2.0.
