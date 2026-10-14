Version: NAFATH-V4
Track: Cybersecurity

Overview
A national service provider depends on a connected technology ecosystem, so security must be considered across the entire software supply chain. The Software field explains how secure configuration and secret management reduce the risk of exposing sensitive information. AI security addresses attacks that can manipulate model inputs or corrupt training data. Mobile application security uses structured verification standards to identify weaknesses before applications reach users. Networking security helps protect internet traffic from malicious route changes, while cybersecurity practices support the identification and remediation of vulnerabilities in software components. Finally, a Software Bill of Materials (SBOM) provides visibility into the components used to build and deliver software. Together, these six fields help organisations understand dependencies, reduce risks, and make informed decisions to protect the confidentiality, integrity, and availability of essential digital services.

Software
Secrets such as API keys, passwords, and access tokens should not be hard-coded into source code or committed to a public repository. They should be stored in an approved secrets manager or secure environment configuration, with access restricted to authorised users and services. Organisations should also rotate exposed credentials, use least-privilege permissions, and scan repositories for accidentally committed secrets. These practices reduce the risk of unauthorised access to systems and data.

Source: OWASP, Secrets Management Cheat Sheet — https://cheatsheetseries.owasp.org/cheatsheets/Secrets_Management_Cheat_Sheet.html



AI
AI systems can be attacked through techniques such as data poisoning, where an attacker manipulates training data, and prompt injection, where malicious instructions attempt to influence a model's behaviour. Defences include validating data sources, limiting model permissions, separating trusted instructions from untrusted content, testing against adversarial inputs, and monitoring system behaviour. No single control prevents every AI attack, so organisations should use layered security measures.

Source: OWASP, Top 10 for Large Language Model Applications — https://genai.owasp.org/llm-top-10/



Mobile
The OWASP Mobile Application Security Verification Standard (MASVS) provides a framework for assessing mobile application security. It covers areas such as secure storage, cryptography, authentication, network communication, platform interaction, and resilience against tampering. Development teams can use MASVS requirements to plan security tests and identify weaknesses before release. The standard supports a systematic assessment rather than relying only on informal testing.

Source: OWASP, Mobile Application Security Verification Standard — https://mas.owasp.org/MASVS/

Networking

Cybersecurity

Data

Misconception in My Track

Open Question
