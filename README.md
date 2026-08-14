## Samuel Boisneault

Cybersecurity engineering student at **ESIEE Paris** (5th year, SecNumedu-accredited by ANSSI).
Looking for a **6-month final-year internship starting February 2027** — application security, DevSecOps or cloud security.

I write backend code, and I am moving toward securing it. Most of what I know about
application security, I learned by instrumenting systems that were not designed to be
instrumented, and paying attention to what fell out.

### Currently

Working through the [PortSwigger Web Security Academy](https://portswigger.net/web-security)
labs and keeping notes in **[websec-labs](https://github.com/ElionSm/websec-labs)** —
SQL injection, access control, SSRF, deserialization.

### Internship at Orange — May to August 2026

Backend Java team, on applications that matter to the business.

I designed and industrialised an internal platform that automates non-regression test
campaigns: Java engine, REST API, web UI for the test repository, campaign dashboard,
wired into GitLab CI/CD and deployed on a PaaS. Alongside it, a Go service that receives
OpenTelemetry traces and turns them into artifacts the pipeline can actually consume —
the facade holds the only public entry point, while the collector and the file writing
stay local to the instance.

While instrumenting a target application, I found a vulnerability and took it end to end:
impact analysis, fix, configuration hardening, and a written analysis for the team. It
confirmed the direction I already wanted, and I went on to own the platform's security
work — a STRIDE threat model mapped to OWASP Top 10, CWE and CAPEC, secret handling in
logs and storage, strict TLS certificate validation, data purges that dry-run by default,
and supply-chain checks that fail the build when a third-party binary's SHA-256 does not
match the pinned value.

The lesson I keep from it: a control that does not produce a decision has produced
nothing. A checksum that is merely logged is not a control; one that stops the build is.

### Tools I have actually used

`Java 17` `Spring Boot` `Go` `Python` `Bash` `SQL` `Angular`
`GitLab CI/CD` `Docker` `AWS` `Cloud Foundry` `MongoDB` `OpenTelemetry` `Nginx`
`OWASP Top 10` `OWASP ASVS` `STRIDE` `ISO/IEC 27001`

### Elsewhere

[LinkedIn](https://www.linkedin.com/in/samuel-boisneault) · samuelboisneault.pro@gmail.com
