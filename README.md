# F5 Secure Cloud AS3 Baselines

- [Secure Cloud Computing Architecture Baseline](sccaBaseline.json) - AS3 v3.5.8


- AS3 Creates:
  - Common/Shared
    - Shared AFM policy
    - Shared ASM policy [Based on DevCentral policies](https://github.com/f5devcentral/f5-asm-policy-templates "f5DevCentral")
    - Shared bot defense policy
    - Shared logging profiles (asm/afm/bot)
    - Shared Client SSL
  - mgmt/admin
    - 80 listner azure health monitor
    - ssh pool
    - rdp listner 
  - Example/exampleApp
    - https service
    - http redirect
    - l4 service
