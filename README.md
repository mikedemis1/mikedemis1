## Michail Demis

Computer engineering graduate from the University of Patras, working on cloud
and platform security. I build things, try to break them, and write down what
actually happened.

Currently: detection engineering on AWS, and a runtime authorisation gateway for
tool-using LLM agents, which is also the subject of a paper in progress with the
University of Patras.

**Working with:** AWS, Terraform, Kubernetes, Python, OPA/Rego, GitHub Actions, Sigma, KQL

### Projects

**[novapay-security-infra](https://github.com/mikedemis1/novapay-security-infra)**
A three-account AWS organisation in Terraform: service control policies, an
organisation CloudTrail, a hardened Kubernetes workload, and a compliance
pipeline that blocks non-conforming infrastructure before it applies. Every
control is read back out of AWS and recorded in `evidence/`, including the ones
that turned out not to work.

**[geo-ads-security-platform](https://github.com/mikedemis1/geo-ads-security-platform)**
Real-time geo-targeted ad platform, my diploma thesis, graded 10/10. FastAPI and
PostGIS with JWT scopes, HMAC-signed WebSocket messages, anti-replay, rate
limiting, and a hybrid rule and Z-score detection engine. An independent review
found a real authentication defect in it; the fix and its regression tests are
in the repository.

**[tool-boundary-monitor](https://github.com/mikedemis1/tool-boundary-monitor)**
Research project on where authorisation belongs when an LLM agent calls tools.
Threat model for indirect prompt injection, and three scoring defects found in
the AgentDojo benchmark while reading its source.

**[aws-secure-landing-zone-terraform](https://github.com/mikedemis1/aws-secure-landing-zone-terraform)**
Where I started. VPC design, private access through SSM Session Manager with no
SSH and no public IPs, log archive, CloudTrail. Nine lessons written down as I
hit them.

### Elsewhere

[LinkedIn](https://www.linkedin.com/in/michalis-demis/) · Greek (native), English (C2), French (B1)
