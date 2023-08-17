# BCPMeta

## Dataset Structure
We use Google Workspace as one example:
1. add_on_info.txt contains all related information descripted in paper
2. review is arranged in dropbox [link], for indexing purpose, we use the processed url as the review file name. For application with url https://workspace.google.com/marketplace/app/zoho_sign_for_gmail/227700145400, just replace the `://` with `-` and `/` with `.`, then add '.json' as file suffix, will get `https-workspace.google.com.marketplace.app.zoho_sign_for_gmail.227700145400.json`.  in python, you can use
   ``` json_file_name = url.replace('://', '-').replace('/', '.') +'.json'  ```
