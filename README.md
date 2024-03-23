# RNIST 800-53 Compliance Implementation Framework

## In This Project:
1. NIST 800-53 Compliance Enablement
  - Thoroughly acquaint stakeholders with the intricacies of NIST 800-53 standards and their significance.
  - Identify and delineate NIST 800-53 controls pertinent to the organizational context.
  - Formulate a dedicated team entrusted with orchestrating NIST 800-53 compliance initiatives.
2. System Compliance Assessment
  - Execute a comprehensive evaluation of existing systems vis-à-vis NIST 800-53 stipulations.
  - Discern discrepancies and areas of non-compliance.
  - Strategically prioritize compliance endeavors predicated on meticulous risk assessments and systemic criticality.
 
3. Compliance Enforcement Measures
  - Devise a meticulous blueprint delineating actionable steps to rectify identified gaps and deficiencies.
  - Implement requisite security protocols and measures in alignment with NIST 800-53 guidelines.
  - Methodically document all interventions undertaken to fortify the system, ensuring auditable and traceable processes.
  - Deliver targeted training sessions to pertinent stakeholders, fostering a robust understanding of NIST 800-53 compliance imperatives.
4. Pre- and Post-Implementation Comparison
  - Undertake periodic evaluations to juxtapose the system's compliance status pre- and post-implementation.
  - Gauge the efficacy of deployed controls in bolstering security posture and achieving NIST 800-53 compliance benchmarks.
  - Document tangible enhancements and discernible insights for future reference and continuous ameliorative efforts.
5. Continuous Monitoring and Refinement
  - Institute a vigilant regime for ongoing monitoring of compliance status, proactively identifying deviations and vulnerabilities.
  - Regularly update security protocols in response to evolving threats and regulatory mandates.
  - Convene routine audits and assessments to corroborate sustained adherence to NIST 800-53 standards.
  - Cultivate an ethos of perpetual improvement and preemptive risk management across the organizational spectrum.
6. Documentation and Reporting Integrity
  - Maintain meticulous records cataloging all facets of NIST 800-53 compliance endeavors, encompassing policies, procedures, and implementation evidence.
  - Furnish regular compliance reports delineating adherence to NIST 800-53 standards, tailored for internal stakeholders, regulatory bodies, and audit scrutiny.
7. Review and Audit Orchestration
  - Orchestrate scheduled reviews and audits of the NIST 800-53 compliance framework to validate efficacy and discern opportunities for optimization.
  - Assimilate feedback gleaned from audits and assessments, iteratively refining and augmenting the compliance framework to align with evolving exigencies.

## The system prior to compliance.
![46](https://github.com/AndrewTanga/Regulatory-compliance---NIST-800-53/assets/93886645/c9419953-c73c-4ae3-933b-cc80fbe75615)

Implementing NIST 800-53: SC-7 Boundary Protection
![SC - 7](https://github.com/AndrewTanga/Regulatory-compliance---NIST-800-53/assets/93886645/ab3bdfa4-0684-4476-a4fd-856431730d47)
![Vulnerability exlorations](https://github.com/AndrewTanga/Regulatory-compliance---NIST-800-53/assets/93886645/442841ac-2226-4f11-a5f0-ae7d323c4a08)

Vulnerability: Subnets should be associated with a network security group

Remediation Steps:
1. Select a subnet to enable NSG on.
2. Click the 'Network security group' section.
3. Follow the steps and select an existing network security group to attach to this specific subnet.

After subnet implementation

![After submitting subnet](https://github.com/AndrewTanga/Regulatory-compliance---NIST-800-53/assets/93886645/4eeb6d9d-45ab-4ce0-b291-98d3366f9a0f)

Vulnerability: Storage account should use a private link connection
Remediation Steps:
1. In the Azure portal, open storage account.
2. From the left sidebar, select 'Configuration'.
3. Make sure 'Allow Blob public access' i sdisabled.
4. From the left sidebar, select 'Networking'.
5. Disable Public network access and save
6. Add 'Private endpoint' and config it correcrly. Make sure vnet and subnet is correct, private IP configuration - Dynamically alloctae IP, DNS(for FQDN)

Vulnerability: Storage accounts should restrict network access using virtual network rules
Remediation Steps: 
1. In the Azure portal, open storage account.
2. From the left sidebar, select 'Networking'.
3. From the 'Allow access from' section, select 'Selected networks'.
4. Add a Virtual network under the 'Virtual networks' section. Do not add allowed IP ranges/ or addresses in the firewall. This is to prevent public IPs from accessing your storage account.

Vulnerability: Access to storage accounts with firewall and virtual network configurations should be restricted
Remediation Steps:
1. In storage account, go to 'Firewalls and virtual networks'.
2. Under 'Allow access from', choose 'Selected networks'.
3. Configure the relevant virtual networks and IP ranges that should be allowed to access your storage account.
4. Configure "Allow trusted Microsoft services to access your storage account".
 





