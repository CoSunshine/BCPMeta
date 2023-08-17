# BCPMeta

## Dataset Structure
We use Google Workspace as one example:
1. add_on_info.txt contains all related information (except for review) descripted in paper, stored in json object for each application. 
2. review is arranged in dropbox [https://www.dropbox.com/sh/041sfcsrtf773j5/AAB3JciH7JXwlCfs4HpDPrOea?dl=0], for indexing purpose, we use the processed url as the review file name. For application with url https://workspace.google.com/marketplace/app/zoho_sign_for_gmail/227700145400, just replace the `://` with `-` and `/` with `.`, then add `.json` as file suffix, will get `https-workspace.google.com.marketplace.app.zoho_sign_for_gmail.227700145400.json`.  in python, you can use

   ```

   json_file_name = url.replace('://', '-').replace('/', '.') +'.json'

   ```

## Metadata:

```json
{
  "add_on_url": "https://workspace.google.com/marketplace/app/%C2%B5funds/274036499952",
  "name": "\u00b5Funds",
  "short_des": "\u00b5Funds is a Google Sheets add-on that allows to import data of your mutual funds directly from Morningstar, only with their ISINs.",
  "developer_infos": {
    "not": "http://www.mufunds.com/",
    "Learn more about the developer's support policy": "https://github.com/joseballester/muFunds/issues",
    "Learn more about the developer's privacy policy": "https://www.mufunds.com/privacy.html",
    "Learn more about the developer's terms of service": "https://www.mufunds.com/terms.html",
    "Learn more about reviews": "https://support.google.com/a/answer/12151326?hl=en_US"
  },
  "price": [
    "Not available",
    "Flag as inappropriate"
  ],
  "overview": "\u00b5Funds is a Google Sheets add-on that allows to import data of your mutual funds directly from Morningstar, only with their ISINs.\n\nThanks to \u00b5Funds, you will be able to import an asset's last NAV and its date, currency or expenses ratio, as well as asset category and other attributes from Morningstar and other data sources. By the use of a simple spreadsheet formula, the desired data can be introduced into your document for many purposes, e.g. portfolio supervision and management or investment strategies.\n\nOnce installed, \u00b5Funds is ready to use: after introducing the data attribute and the fund identifier, the information will appear in the selected cell. Funds can be identified by their ISIN (European funds), ticker (American funds) and also by their Morningstar Security ID (all funds and many pension plans). Check the documentation for a complete list of compatible assets, countries and identifiers.",
  "images:": [
    "https://lh3.googleusercontent.com/oKt5hIN-ITLve47-zFvj7Rg4BSrQIm7xelvrTXcQLV9vWnyCYvPsnzYRwgGYhbbVVw3eCrHH=s640-w640-h400"
  ],
  "host_apps": [
    "Google Sheets icon"
  ],
  "permissions": [
    "UKASM;274036499952;2",
    "kATLae;_;8",
    "gl8KFd;https://www.googleapis.com/auth/userinfo.email;9",
    "gl8KFd;https://www.googleapis.com/auth/userinfo.profile;10"
  ],
  "perm_text": [
    "See your primary Google Account email address",
    "See your personal info, including any personal info you've made publicly available"
  ],
  "rating_avg": "4.2",
  "rating_worst": "0",
  "rating_best": "5",
  "rating_persons": "72",
  "download_num": "7K+",
  "last_updated": "Listing updated:October 6, 2022"
}

```


###  review
```json

{
 "Name": "Jai Kumar",
 "reviewTime": "April 10, 2019",
 "review": "It's quite helpful for me. Now I can access and search answers to important customer questions with Ease.",
 "grade": "User Rating: 5 stars",
 "userImg": "https://lh3.googleusercontent.com/a-/AD_cMMROYuLsu7fqsBWL2S5RRxNLrUbRtD1sqlmvUwgy30F7z0im=s40-c-k"
}
{
 "Name": "A User of Zuzu AI for Gmail™",
 "reviewTime": "May 20, 2019",
 "review": "Where to find Zuzu AI: Knowledge Assistant for Gmail\nOpen a message in Gmail web or on your Android phone to find applicable add-ons.",
 "grade": "User Rating: 5 stars",
 "userImg": "https://lh3.googleusercontent.com/a-/AD_cMMRu5Zy8Z7d4Oe0uOh3FbIUoUWPmGH6fuHmHrGdrXbgrkw=s40-c-k"
}
{
 "Name": "A User of Zuzu AI for Gmail™",
 "reviewTime": "April 10, 2019",
 "review": "Great add-on for Sharing Knowledge.",
 "grade": "User Rating: 5 stars",
 "userImg": "https://lh3.googleusercontent.com/a/default-user=s40-c-k"
}
{
 "Name": "A User of Zuzu AI for Gmail™",
 "reviewTime": "May 27, 2019",
 "review": "fantastic",
 "grade": "User Rating: 4 stars",
 "userImg": "https://lh3.googleusercontent.com/a/default-user=s40-c-k"
}
{
 "Name": "A User of Zuzu AI for Gmail™",
 "reviewTime": "April 10, 2019",
 "review": "Really Helpful!!!",
 "grade": "User Rating: 5 stars",
 "userImg": "https://lh3.googleusercontent.com/a/default-user=s40-c-k"
}

```

## Statics Summary:
Application Number: 4462

Application with Review: 3391

