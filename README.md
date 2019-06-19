# gsheet-integration
In this repo I'll create an integration between a java client and the Google Sheets API just to have a personal budget tool with a BD in Google Sheets.

Requirements:
- Install Gradle
- Enable Google Sheets API and get the required credentials
```json
{
    "installed": {
        "client_id": "*****.apps.googleusercontent.com",
        "project_id": "quickstart-*****",
        "auth_uri": "https://accounts.google.com/o/oauth2/auth",
        "token_uri": "https://oauth2.googleapis.com/token",
        "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
        "client_secret": "*****",
        "redirect_uris": [
            "urn:ietf:wg:oauth:2.0:oob",
            "http://localhost"
        ]
    }
}
```
- Include the required api libraries from google.
    - com.google.api-client:google-api-client
    - com.google.oauth-client:google-oauth-client-jetty
    - com.google.apis:google-api-services-sheets
       
#####How to get the Google Sheet ID?
* You just need to go the the sheet in your browser
* The URL should looks like:  
`https://docs.google.com/spreadsheets/d/${SHEET_ID}/edit#gid=0`  
* Just copy and paste the SHEET_ID part of the url.   
       
TODOs:
- Update to Kotlin DSL 