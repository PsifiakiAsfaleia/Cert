# Chapter 0:-

# Compare and contrast various types of security controls.  

## Part 1: Control Categories ( How they are implemented ):-
Control categories define the nature of the control based on who or what enforces it.

### 1. Technical controls ( Logical Controls ):-
These are safeguards implemented through hardware, software, or firmware. They rely on technology to enforce security policies automatically without human  intervention.

- **Key Characteristics:** Automated, system-enforced, and code-based.

- **Deep-Dive Examples:**

    - **Firewalls and ACLs:** Automatically blocking unauthorized network traffic based on protocols and IP addresses.

    - **Encryption ( AES-256 ):** Ensuring data confidentiality at rest or in transit by transforming plaintext into ciphertext.

    - **Intrusion Prevention System (IPS ):** Actively dropping malicious packets on a network.

    - **Multi-Factor Authentication ( MFA ):** Software-driven validation of identity via tokens, biometrics, or passwords.

### 2. Managerial Controls ( Administrative Controls ):-
These focus on the oversight, selection, and management of security measures. They are driven by organizational leadership, policy, and strategy to guide human behavior and corporate governance.

- **Key Characteristics:** Policy-driven, compliance-oriented, and strategic.

- **Deep-Dive Examples:**

    - **Formal Security Policies:** Documented rules like an Acceptable Use Policy ( AUP ) or Password Policy.

    - **Risk Assessments:** Regularly scheduled processes to identify vulnerabilities, quantify threats, and choose risk response.

    - **Business Continuity and Disaster Recovery ( BC/DR ) Planes:** Management frameworks detailing how the company will survive a catastrophic outage.

    - **Vendor Risk Management:** Establishing security criteria that third-party contractors must legally satisfy.

### 3. Operational Controls:-
These are security measures executed by people rather than systems. They integrate security into the day-to-day practices, routines, and operations of an organization.

- **Key Characteristics:** Human-centric, process-dependent, and daily routine-focused.
- **Deep-Dive Examples:**

    - **Security Awareness Training:** Educating employees on how to spot phishing emails and social engineering tactics.

    - **Configuration Management & Change Control:** Human review boards approving system modifications before they go live to prevent downtime.

    - **Media Sanitation:** Safely shredding paper documents or using software to completely wipe hard drives before disposal.

    - **Incident Response steps:** The physical and intellectual actions taken by a security team during an active breach.

### 4. Physical Controls:-
These are tangible, real-world measures designed to protect physical spaces, assets, and personnel from unauthorized access or environmental hazards.

- **Key Characteristics:** Concrete, touchable, and geographically bound.

- **Deep-Dive Examples:**

    - **Perimeter Barriers:** Fences, Barricards, and vehicle bollards to stop forced entry.

    - **Access Restrictors:** Badges, physical locks, mantraps, and biometric turnstiles.

    - **Environmental Controls:** Fire suppression systems ( FM-200 ), HVAC systems, and backup generators.

    - **Surveillance & Guarding:** Human security guards and closed-circuit Television ( CCTV ) cameras.

## Part 2: Control Types ( What they are designed to do ):-
Control types classify safeguards based on their functional objective and their timing relative to a security incident ( before, during, or after ).

> [ Directive ] → [ Deterrent ] → [ Preventive ] → ( INCIDENT ) → [ Detective ] → [ Corrective/Compensating ]

### 1. Directive Controls:-
These dictate proper behavior and define what actions are allowed or prohibited within an organization. They form the foundation “rules of engagement” before any other control is built.

- **Functional Goal:** To specify compliance and enforce rules.

- **Deep-Dive Examples:**

    - **Standard Operating Procedures ( SOPs ):** Step-by-step guides on how tasks must be securely performed.

    - **Regulations and Laws:** External directives like GDPR, HIPAA, OR PCI-DSS.

    - **Signs:** A physical sign posted on a gate that states “Authorized Personnel Only.”

### 2. Deterrent Controls:-
These aim to discourage a potential attacker or insider from attempting a malicious action by making the effort, risk, or consequences appear too high. They appeal to the adversary’s psychological risk calculus.

- **Functional Goal:** To psychologically dissuade or scare off an attacker.

- **Deep-Dive Examples:**

    - **Visible Security Cameras:** An attacker sees the camera and chooses an easier target to avoid being caught.

    - **Warning Banners:** A login screen massage starting: “All activity is monitored. Unauthorized access will be prosecuted.”

    - **Lighting:** Well-lit building exteriors that strip away an intruder’s cover of darkness.

### 3. Preventive Controls:-
These actively stop a security incident from occurring in the first place. They act as a hard barrier that cannot easily be bypassed by simple intent.

- **Functional Goal:** To block or intercept an attack before damage happens.

- **Deep-Dive Examples:**

    - **Firewalls:** Outright blocking unauthorized incoming ports.

    - **Smart Cards/Keypads:** Physically blocking an unauthorized body from opening a data center door.

    - **Input Validation:** Code that strips away malicious SQL injection strings before they reach a database.

### 4. Detective Controls:-
These identify and log security incidents, irregularities, or unauthorized activities while they are happening or after they have occurred. They provide visibility when preventive controls fail.

- **Functional Goal:** To discover, alert, and document anomalous activity.

- **Deep-Dive Examples:**

    - **Intrusion Detection Systems ( IDS ):** Monitoring traffic and triggering alarm when a known attack signature is found.

    - **Log Review & SIEM:** Analyzing system events logs to find indicators of compromise ( IOCs ).

    - **Motion Detectors:** Alarms that trigger when movement is found in a restricted area after hours.

    - **Audit Trails:** Reviewing financial or user-privilege histories to spot unauthorized changes.

### 5. Compensating Controls:-
These are alternative security measures put in place when a primary control is impossible, too expensive, or impractical to implement. They must provide an equivalent level of defense.

- **Functional Goal:** To temporarily or permanently fill a gap left by missing primary control.

- **Deep-Dive Examples:**

    - **The Legacy Server Dilemma:** An old manufacturing machine requires Windows XP to run and cannot be patched ( missing preventive control ). Compensating Control: Isolate the machine entirely from the internet on an air-gapped VLAN and monitor it with an aggressive IDS.

    - **Single-Symptom MFA Failure:** An application doesn’t support MFA. Compensating Control: Enforce exceptionally long, rotating passwords coupled with strict IP-address whitelisting.

## #Summary Matrix For Quick Review:-

| Control Name | Category | Type | Why it fits |
| :----------- | :------- | :--- | :---------- |
| Security Camera | Physical | Deterrent/Detective | It is a tangible object ( Physical ) that scares intruders ( Deterrent ) and records them if they enter ( Detective ). |
| Firewall rule | Technical | Preventive | It is software/hardware-based ( Technical ) and actively blocks traffic ( Preventive ). |
| AUP Policy Sign-off | Managerial | Directive | It is a leadership-driven rule ( Managerial ) that tells employees how to behave ( Directive ). |
| Air-Gapping a Legacy OS | Technical/Operational | Compensating | It uses configuration changes ( Technical ) to substitute for a missing patch ( Compensating ). |





