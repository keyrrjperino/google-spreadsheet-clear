# Google Spreadhsheet Api - Clear Data

A [Supercode](http://gosupercode.com) function that clear data on google spreadsheet.
Still developing for other methods of google spreadsheet api.

## Server Usage

[Supercode](http://gosupercode.com) SDK will be available after the launch.

```
import supercode
import pprint

credentials_json_data = {}

response = supercode.call(
    "super-code-function",
    "your-supercode-api-key",
    method_name,
    credentials_json_data,
    spreadsheet_id,
    range_name
)

pprint(response)
```

## Testing on Command Line
`python test.py --help`

example:

    json_data='{
      "type": "service_account",
      "project_id": "symph-git-hooks",
      "private_key_id": "",
      "private_key": "",
      "client_email": "",
      "client_id": "",
      "auth_uri": "",
      "token_uri": "",
      "auth_provider_x509_cert_url": "",
      "client_x509_cert_url": ""
    }'
    
    python test.py --method_name="update" --credentials_json_data=$json_data --spreadsheet_id="<your spreadsheet id>" --range_name="Sheet1\!A1:B1"


**Note:** Supercode has not been launched yet. This is for internal testing only.
