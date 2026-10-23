## Michail Demis

Computer engineering graduate from the University of Patras, looking for a
junior role in cloud security, cloud engineering or security engineering. I
build things, try to break them, and write down what actually happened.

Currently: studying for AZ-104 (Microsoft Azure Administrator).

**Working with:** AWS, Azure, Terraform, Kubernetes, Python, OPA/Rego, GitHub Actions, Sigma, KQL

### Projects

Each one says what broke and what the wrong first attempt was. If you open only
one, open the first and watch its video.

**[assume-hijacked](https://github.com/mikedemis1/assume-hijacked)**
A support chat agent for a made-up electricity supplier, built on the assumption
that the model is already hijacked. The model holds no password, no database
connection and no route to the internet; every action it asks for goes through
checks that ignore its words. Kubernetes with Cilium default-deny between every
service, a risk engine that sends money moves to a human, 717 tests. The
video shows Claude refusing on its own, then a scripted hijacked model trying
four attacks that all stop, and 20 connections out of a tool pod that all time
out. The Terraform for AKS with Kata nodes was applied once on Azure; the app
has not run there yet.

**[novapay-security-infra](https://github.com/mikedemis1/novapay-security-infra)**
A three-account AWS organisation in Terraform: service control policies, an
organisation CloudTrail, a hardened Kubernetes workload, and a compliance
pipeline that blocks non-conforming infrastructure before it applies. Every
control is read back out of AWS and recorded in `evidence/`, including the two
guardrails of five that turned out never to have been applied at all.

**[geo-ads-security-platform](https://github.com/mikedemis1/geo-ads-security-platform)**
Real-time geo-targeted ad platform, my diploma thesis, graded 10/10. FastAPI and
PostGIS with JWT scopes, HMAC-signed WebSocket messages, anti-replay, rate
limiting, and a hybrid rule and Z-score detection engine. An independent review
found a real authentication defect in it; the fix and its regression tests are
in the repository.

**[tool-boundary-monitor](https://github.com/mikedemis1/tool-boundary-monitor)**
Research on where authorisation belongs when an LLM agent calls tools. An inline
gateway decides on a proposed call before it executes: with nothing checking, 27
of 27 scripted attacker goals succeed; under the full task contract, none do,
and 3 of 27 benign tasks stop for a human, which is reported in the same table.
Two defects in the benchmark's own scoring were found by reading its source, and
reported, not patched.

**[aws-secure-landing-zone-terraform](https://github.com/mikedemis1/aws-secure-landing-zone-terraform)**
Where I started. Private-subnet access over SSM Session Manager with no SSH, no
NAT gateway and no public IP, proven end to end: IMDSv1 refused, the outbound
request timing out, packages still arriving through an S3 gateway endpoint. Nine
lessons written down as I hit them.

### Elsewhere

[LinkedIn](https://www.linkedin.com/in/michalis-demis/) · Greek (native), English (C2), French (B1)
