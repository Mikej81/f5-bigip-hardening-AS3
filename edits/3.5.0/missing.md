waf_asm
-------
reqires xml copied to device first
`
curl -vk https://raw.githubusercontent.com/Mikej81/f5-securecloud-AS3/master/asm/13.1/sccaBaselineASMPolicy.xml -o /shared/vadc/azure/waagent/custom-script/download/0/sccaBaselineASMPolicy.xml

/shared/vadc/azure/waagent/custom-script/download/0/sccaBaselineASMPolicy.xml
`
file urls: "https://raw.githubusercontent.com/Mikej81/f5-securecloud-AS3/master/asm/13.1/sccaBaselineASMPolicy.xml"

protocol_inspection:
--------------------

tmsh modify security firewall policy Shared/sccaBaselineAFMPolicyHTTP rules modify { allow_all { protocol-inspection-profile protocol_inspection }}


modify security firewall policy Shared/sccaBaselineAFMPolicyHTTP rules modify { allow_all { protocol-inspection-profile protocol_inspection_http }}

IPI
---

done via irule still