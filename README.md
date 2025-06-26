# CSEQL-Llama
This is an official repository for CSEQL-Llama. You can access SynCEQL  dataset and CSEQL-Llama models.

## Dataset
SynCEQL dataset is available at [SynCEQL.json](./SynCSEQL.json). 

It's a json file with the following format:
```json
[
    {
        "db_id": "FOFA",
        "query": "app=\"Microsoft-Exchange\" && cert.is_expired=true && cname_domain=\"siteforce.com\"",
        "query_toks": [
            "app",
            "=",
            "\"Microsoft-Exchange\"",
            "&&",
            "cert.is_expired",
            "=",
            "true",
            "&&",
            "cname_domain",
            "=",
            "\"siteforce.com\""
        ],
        "query_toks_no_value": [
            "app",
            "=",
            "\"microsoft-exchange\"",
            "&&",
            "cert.is_expired",
            "=",
            "true",
            "&&",
            "cname_domain",
            "=",
            "\"siteforce.com\""
        ],
        "question": "Discover cyberspace assets with Microsoft-Exchange application, expired certificates, and the main domain resolved from CName is 'siteforce.com'.",
        "question_toks": [
            "Discover",
            "cyberspace",
            "assets",
            "with",
            "Microsoft-Exchange",
            "application,",
            "expired",
            "certificates,",
            "and",
            "the",
            "main",
            "domain",
            "resolved",
            "from",
            "CName",
            "is",
            "'siteforce.com'."
        ],
        "cot": ""
    },
    ......
]
```