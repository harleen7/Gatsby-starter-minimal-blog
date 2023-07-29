---
title: What's UULE Parameter?
date: "2023-07-29T22:16:13.284Z"
description: "The uule paramter is the parameter often used in various google serp location changer tools. Learn more about it here!"
---

The "uule" parameter is a special query parameter used in Google search URLs. It is primarily employed to encode the geographic location and language settings for the search query, enabling Google to return more relevant and localized search results.

## Purpose of the uule Parameter in Google SERP

The purpose of the "uule" parameter is to help users or developers to perform location-specific searches directly from the URL, rather than relying solely on the default location settings of the user's IP address. By including the "uule" parameter in the URL, users can see search results as if they were conducting the search from a specific location, regardless of their physical location.

## Format of the uule Parameter

The format of the "uule" parameter is a Base64-encoded string, and it typically contains information about the geographic location and language settings. The specific format of the parameter is not publicly documented by Google, and it's subject to change. As of my last update in September 2021, the "uule" parameter can be generated using various online tools, but it's essential to use such tools from reputable sources.

## Example Usage of the uule Parameter

Here's a simplified example of how the "uule" parameter works:

Suppose you want to search for "restaurants" in the city of "New York" and prefer to see the results as if you were conducting the search from "New York, USA." You can construct the Google search URL with the "uule" parameter as follows:


[https://www.google.com/search?q=restaurants&uule=w+CAIQICIITmV3IFlvcms](https://www.google.com/search?q=restaurants&uule=w+CAIQICIITmV3IFlvcms)

In this example, "w+CAIQICINVW5pdGVkIFlvcms" is the uule representation of the location "New York, USA." It consists of 3 things:
1. A fixed paramter which is w+CAIQI
2. The length of the string called New York
3. The base-64 encoded city name. 

When Google receives this request, it uses the "uule" parameter to understand that the search should be location-specific to "New York," and it will return results accordingly.

But, keep in mind, Google doesn't officially document this stuff, so it might change one day. So, be careful if you're building something serious with it.

In summary, the "uule" parameter is a useful tool for generating location-specific search URLs for Google. However, since it's not officially documented and could change in the future, developers should exercise caution and be prepared for its potential unavailability.

This was written by ChatGPT but fact-checked and edited by Harleen Sandhu. (See About me)
