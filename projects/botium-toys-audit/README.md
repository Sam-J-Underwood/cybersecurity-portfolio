# Botium Toys: Internal Security Audit


## Project overview


This Google Cybersecurity course exercise examines the security posture of Botium Toys, a fictional toy retailer with a storefront, warehouse, and growing online business. The audit covers its security program, including equipment, internal network, systems, and data.


My task was to review the supplied scope, goals, and risk assessment report, then complete a controls and compliance checklist. The analysis below reflects the supplied scenario rather than independent testing of live systems.


## Approach


1. Reviewed the audit scope, goals, current assets, and risk assessment.
2. Compared the report's evidence with the control categories reference.
3. Recorded whether each control and compliance practice was currently in place.
4. Identified improvements based on the gaps in the report.


## Key findings


The supplied report rates risk at 8 out of 10. Major gaps include overly broad access to sensitive information, missing encryption, no critical-data backups, and no disaster recovery plan. Existing protections include a firewall, antivirus software, physical security measures, and controls supporting data integrity and availability.


## Controls assessment

Answers follow my revised checklist. For password policies and legacy-system monitoring, “No” reflects inadequate implementation, even though some measures exist.


| Control | In place? | Evidence from the scenario |
| --- | --- | --- |
| Least privilege | No | All employees can access internally stored data. |
| Disaster recovery plans | No | No disaster recovery plans are in place. |
| Password policies | No | A policy exists, but its weak requirements do not adequately meet the control objective. |
| Separation of duties | No | The report states that this control has not been implemented. |
| Firewall | Yes | Traffic is filtered using defined security rules. |
| Intrusion detection system | No | No IDS has been installed. |
| Backups | No | Critical data is not backed up. |
| Antivirus software | Yes | Installed and monitored regularly. |
| Legacy-system monitoring, maintenance, and intervention | No | Some monitoring and maintenance occur, but there is no regular schedule and intervention procedures are unclear. |
| Encryption | No | Customer payment information is not encrypted internally. |
| Password management system | No | No centralized system is in place. |
| Locks | Yes | Offices, storefront, and warehouse have sufficient locks. |
| CCTV surveillance | Yes | Surveillance is up to date. |
| Fire detection and prevention | Yes | Functioning systems are present. |


## Compliance checklist assessment


These judgments answer the course checklist using the fictional report; they do not constitute a formal compliance determination.


| Checklist area | Practice | Met? |
| --- | --- | --- |
| PCI DSS | Access to card information restricted to authorized users | No |
| PCI DSS | Secure internal storage, acceptance, processing, and transmission of card information | No |
| PCI DSS | Encryption of card transaction data | No |
| PCI DSS | Secure password management policies | No |
| GDPR | EU customer data kept private and secure | No |
| GDPR | The scenario's stated 72-hour customer notification plan | Yes |
| GDPR | Data properly classified and inventoried | No |
| GDPR | Privacy policies and processes for documenting and maintaining data | Yes |
| SOC | User access policies established | No |
| SOC | Sensitive data kept confidential | No |
| SOC | Data integrity maintained | Yes |
| SOC | Data available to authorized individuals | Yes |


## Recommendations

Botium Toys should prioritize restricting access to sensitive customer and payment information by implementing least privilege and separation of duties. Encryption should also be introduced to protect this information during storage and transmission.

The company should establish regular backups of critical data and a documented disaster recovery plan, with recovery procedures tested regularly. An intrusion detection system should be installed to help identify suspicious network activity.

Existing password policies should be strengthened and supported by a centralized password management system. Legacy systems should have a regular monitoring and maintenance schedule, with clear intervention procedures and assigned responsibilities.

Finally, Botium Toys should complete its asset inventory and classify data by sensitivity to support appropriate protection and compliance practices.

## Reflection


This exercise highlights the difference between a control existing and being effective: password policies and legacy-system monitoring exist in limited form, but are assessed as “No” in my revised checklist because they are not adequately implemented. It also distinguishes availability from confidentiality. The report confirms that authorized users can access data, even though excessive access creates a separate confidentiality risk.


## Source materials


Google Cybersecurity course activity materials: *Botium Toys: Scope, goals, and risk assessment report*, *Control categories*, and *Controls and compliance checklist*. Findings are based on the supplied version of those materials.

