# F5 BIG-IP Hardening AS3 Baselines

This repository contains a select of AS3 example baselines tied to Government BIG-IP Hardening Requirements, as well as other application hardening examples for F5 Secure Cloud Architectures.  

Folder Structure:

- dist
  - arm - Azure Resource Manager Examples
    - version
  - cft - AWS Cloud Formation Templates Examples
  - terraform - Terraform Template Examples

- [ARM Secure Cloud Computing Architecture Baseline](https://raw.githubusercontent.com/Mikej81/f5-securecloud-AS3/master/dist/arm/3.16.0/sccaBaseline.json) - AS3 v3.16.0

- These AS3 Examples Create the following objects:
  - Common/Shared
    - Shared AFM policy
    - Shared ASM policy [Based on DevCentral policies](https://github.com/f5devcentral/f5-asm-policy-templates "f5DevCentral")
    - Shared bot defense policy
    - Shared logging profiles (asm/afm/bot)
    - Shared Client SSL
  - mgmt/admin
    - 80 listener azure health monitor
    - ssh pool
    - rdp listener
  - Example/exampleApp
    - https service
    - http redirect
    - l4 service
