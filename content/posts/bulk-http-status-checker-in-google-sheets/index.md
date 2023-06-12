---
title: Checking HTTP Status in Google Sheets Using Custom Formula with AppScript
date: 2023-06-12
slug: /checking-http-status-google-sheets-custom-formula-appscript
description: Here's an easy script you use add in AppScript in Google Sheets to check HTTP Status Codes of URLs in bulk
tags:
  - Tutorial
banner: ./banner.jpg
---
There are many HTTP Status Code checkers out there that can do the job for you as well. One of my favorite is http://httpstatus.io/.

There are scenarios where your server blocks any requests made by bots. In those cases, such tools will give you the status code 403 - Forbidden.

In such a case, creating a custom formula in Google sheets for checking HTTP status codes can come to the rescue. Google Sheets is able to check the status codes without getting blocked out by the server is because it will use your IP, hopefully which will not be blocked.

## Steps to check Status Codes in Google Sheets
1. Open AppScript in Google Sheets and Paste the following code

**Javascript Code for Status Codes in Google Sheets
```
function statusCode (url){

   var options = {

     'muteHttpExceptions': true,

     'followRedirects': false

   };

   var url_trimmed = url.trim();

   var response = UrlFetchApp.fetch(url_trimmed, options);

   return response.getResponseCode();

}
```

2. Use this formula in your GoogleSheets to check the Status code:

```
   =statusCode(URL)
```

That's it.
