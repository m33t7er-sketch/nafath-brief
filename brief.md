Version: NAFATH-V4
Track: Cybersecurity

Overview
A national service provider depends on a connected technology ecosystem, so security must be considered across the entire software supply chain. The Software field explains how secure configuration and secret management reduce the risk of exposing sensitive information. AI security addresses attacks that can manipulate model inputs or corrupt training data. Mobile application security uses structured verification standards to identify weaknesses before applications reach users. Networking security helps protect internet traffic from malicious route changes, while cybersecurity practices support the identification and remediation of vulnerabilities in software components. Finally, a Software Bill of Materials (SBOM) provides visibility into the components used to build and deliver software. Together, these six fields help organisations reduce risk and protect essential digital services, including by identifying and remediating critical vulnerabilities such as Log4Shell (CVE-2021-44228).

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
BGP route hijacking occurs when an autonomous system announces incorrect routing information, potentially diverting internet traffic through an unauthorised network. Resource Public Key Infrastructure (RPKI) uses cryptographically signed records to help verify whether an autonomous system is authorised to originate a route. Route Origin Validation can reject invalid origin announcements, but RPKI does not prove the entire network path is legitimate or prevent every routing attack.

Resource: RFC 6811 - BGP Prefix Origin Validation - https://www.rfc-editor.org/rfc/rfc6811



Cybersecurity
Log4Shell (CVE-2021-44228) was a critical vulnerability in Apache Log4j 2, a widely used Java logging library. In affected configurations, an attacker could send crafted input that triggered a JNDI lookup and potentially execute code remotely. Its severity came from the library's widespread use and the possibility of unauthenticated remote exploitation. The main mitigation is to upgrade to a fixed Log4j version and verify that vulnerable copies are no longer present.

Resource: NIST National Vulnerability Database - CVE-2021-44228 - https://nvd.nist.gov/vuln/detail/CVE-2021-44228

Data
A Software Bill of Materials (SBOM) is a structured inventory of the components included in a software product. It helps organisations identify dependencies, investigate vulnerabilities, and determine which products may be affected by a newly disclosed flaw. A useful SBOM records component names, versions, suppliers, unique identifiers, dependency relationships, and information about the document itself. Organisations should keep SBOMs accurate and update them as software changes.

Resource: NTIA - The Minimum Elements for a Software Bill of Materials (SBOM) - https://www.ntia.gov/report/2021/minimum-elements-software-bill-materials-sbom

Misconception in My Track
Log4Shell is sometimes misunderstood as a vulnerability that only affects internet-facing websites. In reality, the risk depends on whether a vulnerable version of Apache Log4j 2 is present and whether an attacker can reach a vulnerable logging path. The vulnerability could allow remote code execution in affected configurations, so organisations must identify vulnerable components across their systems, not just public websites. The NIST National Vulnerability Database entry for CVE-2021-44228 documents the affected versions and vulnerability details, supporting the need to assess exposure and apply fixes.

Open Question
How can organisations reliably identify every vulnerable Log4j instance across legacy systems and third-party software?
