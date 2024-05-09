To update database to the lastest version, run

wpscan --update
Scan installed plugins

wpscan --url http(s)://your-domain.com --enumerate p
Scan vulnerable plugins

wpscan --url http(s)://your-domain.com --enumerate vp
Scan installed themes

wpscan --url http(s)://your-domain.com --enumerate t
Scan vulnerable themes

wpscan --url http(s)://your-domain.com --enumerate vt
Scan user accounts:

wpscan --url http(s)://your-domain.com --enumerate u
Scan vulnerable timthumb files:

wpscan --url http(s)://your-domain.com --enumerate tt
Please note that scanning other’s websites is illegal. Do it only on your own website.

Using WPVulnDB API
By default, WPScan only tells you if there’s vulnerabilities found, but doesn’t show the details of vulnerabilities. You can get a free API token with 50 daily requests by registering at https://wpvulndb.com/users/sign_up.

Once you have created account, you can save the API token in a file. Run the following command to create WPScan configruation file.

nano ~/.wpscan/scan.yml
Put the following lines in the file.

cli_options:
    api_token: YOUR_API_TOKEN
