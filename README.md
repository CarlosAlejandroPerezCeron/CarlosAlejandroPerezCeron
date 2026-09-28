## Carlos Alejandro Perez

Principal Cloud, AI & Identity Security Architect · Bogotá, Colombia

12+ years operating production platforms in regulated financial services, insurance, media and retail. I work where cloud IAM, AI workloads and platform engineering meet: who and what can reach a model, a dataset or a production account, how that access is proven, and how fast a misuse is detected and contained.

Current focus: securing GenAI and agentic workloads (model access control, prompt injection, tool authorization), cloud and workload identity (AWS IAM, Entra ID, OIDC federation), and detection with automated remediation.

### Security tooling

Small, tested CLIs with CI-friendly exit codes. The prompt, secrets, IAM policy and Terraform tools run offline on files; the S3, security group, Lambda and CloudTrail tools read live configuration through boto3 with read-only credentials.

| Repo | What it catches |
| --- | --- |
| [llm-prompt-guard](https://github.com/CarlosAlejandroPerezCeron/llm-prompt-guard) | Prompt injection, jailbreaks, indirect injection in external content, PII and secrets before text reaches an LLM |
| [aws-iam-analyzer](https://github.com/CarlosAlejandroPerezCeron/aws-iam-analyzer) | Wildcard admin, `iam:PassRole` escalation, inline user policies, destructive S3 grants |
| [aws-cloudtrail-analyzer](https://github.com/CarlosAlejandroPerezCeron/aws-cloudtrail-analyzer) | Root usage, console brute force, MFA removal, trail tampering, wildcard IAM changes |
| [aws-secrets-scanner](https://github.com/CarlosAlejandroPerezCeron/aws-secrets-scanner) | Hardcoded AWS keys, private keys, passwords, credentialed DSNs and API tokens, redacted in output |
| [terraform-security-linter](https://github.com/CarlosAlejandroPerezCeron/terraform-security-linter) | Open security groups, public RDS, unversioned S3, IAM wildcards, public EC2 IPs in HCL |
| [aws-s3-security-scanner](https://github.com/CarlosAlejandroPerezCeron/aws-s3-security-scanner) | Public access, missing encryption, versioning and logging gaps, wildcard bucket policies |
| [aws-sg-auditor](https://github.com/CarlosAlejandroPerezCeron/aws-sg-auditor) | SSH/RDP open to the internet, all-traffic rules, internet-exposed ports, default SG misuse |
| [aws-lambda-auditor](https://github.com/CarlosAlejandroPerezCeron/aws-lambda-auditor) | Over-permissioned execution roles, secrets in env vars, deprecated runtimes, no VPC, no DLQ |

### How I work

Controls are enforced where traffic and identity actually flow, measured, and owned by the platform rather than bolted on after release. Every tool here ships with tests and CI; nothing in these repos contains employer code, data or configuration.

[LinkedIn](https://www.linkedin.com/in/carlos-alejandro-perez-ceron-a3b0b6213) · [Email](mailto:ceron8402@gmail.com)
