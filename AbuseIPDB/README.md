https://www.abuseipdb.com/api.html

What this will do:
* Check if an IP has been repoted for malciious behavior (brute force, spam, etc)

---

Check IP
`https://www.abuseipdb.com/check/[IP]/json?key=[API_KEY]&days=[DAYS]`

Check CIDR
`https://www.abuseipdb.com/check-block/json?network=[CIDR]&key=[API_KEY]&days=[DAYS]`

Report IP
`https://www.abuseipdb.com/report/json?key=[API_KEY]&category=[CATEGORIES]&comment=[COMMENT]&ip=[IP]`



### Parameters Explained

| Field        | Required | Default | Example                               | Description                                                                 |
|--------------|----------|---------|---------------------------------------|-----------------------------------------------------------------------------|
| `[IP]`       | Yes      | NA      | `8.8.8.8` / `::1`                      | IPv4 or IPv6 Address                                                        |
| `[DAYS]`     | No       | 30      | `30`                                  | Check for IP Reports in the last 30 days                                   |
| `[API_KEY]`  | Yes      | NA      | `Tzmp1...quWvaiO`                      | Your API Key ([Get an API Key](https://www.abuseipdb.com/account))                                         |
| `[CATEGORIES]` | Yes    | NA      | `10,12,15`                            | Comma delineated list of category IDs ([See all Categories](https://www.abuseipdb.com/categories))            |
| `[COMMENT]`  | No       | blank   | `Brute forcing Wordpress login`       | Describe the type of malicious activity                                    |
| `[CIDR]`     | Yes      | NA      | `207.126.144.0/20`                    | IPv4 Address Block in CIDR notation                                        |
| `verbose` flag | No     | FALSE   | `/json?key=[API_KEY]&days=[DAYS]&verbose` | When set, reports include comments and reporter's user ID (0 = anonymous)  |
