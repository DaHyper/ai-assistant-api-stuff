https://docs.virustotal.com/reference/overview

Scan URL
```
curl --request POST \
     --url https://www.virustotal.com/api/v3/urls \
     --header 'accept: application/json' \
     --header 'content-type: application/x-www-form-urlencoded'
```


Malware Upload (Future Project)

Curl Request (Uploading a File):
```
curl --request POST \
     --url https://www.virustotal.com/api/v3/files \
     --header 'accept: application/json' \
     --header 'content-type: multipart/form-data'
```


Get a crowdsourced Sigma rule object:
```
curl --request GET \
     --url https://www.virustotal.com/api/v3/sigma_rules/id \
     --header 'accept: application/json'
```

Get a crowdsourced YARA ruleset
```
curl --request GET \
     --url https://www.virustotal.com/api/v3/yara_rulesets/id \
     --header 'accept: application/json'
```