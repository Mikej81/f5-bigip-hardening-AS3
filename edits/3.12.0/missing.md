protocol_inspection:
--------------------

tmsh modify security firewall policy Shared/sccaBaselineAFMPolicyHTTP rules modify { allow_all { protocol-inspection-profile protocol_inspection }}


modify security firewall policy Shared/sccaBaselineAFMPolicyHTTP rules modify { allow_all { protocol-inspection-profile protocol_inspection_http }}

Logging:
--------

bot_defense
    logging profile
    "bot_defense" :{
    "class": "Security_Log_Profile",
    "botDefense": {
        "localPublisher": {
            "bigip":"/Common/local-db-publisher"
        },
        "logBotSignatureMatchedRequests": true,
        "logCaptchaChallengedRequests": true,
        "logChallengedRequests": true,
        "logIllegalRequests": true,
        "logLegalRequests": true
    }
},