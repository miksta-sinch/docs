---
title: "Introduction"
excerpt: ""
---
## Overview

Sinch offers a platform for phone number verification. It consists of different software development kits – the Sinch SDKs – that you integrate with your smartphone or web application and cloud based back-end services. Together, they enable SMS and Flash Call verification in your application.

## What are the supported platforms?

When using Sinch for Verification, the Sinch dashboard can provide both SMS and Flash Call verification (on Android mobile devices only).

The Sinch Verification service takes care of all the different steps in a verification process and let developers focus on building great application while easily reinforcing their sign up and login processes.

## What are the different verification services?

The Sinch SDK is currently available for `iOS <verification-ios>`, `Android <verification-android>` and `JavaScript <verification-js>` platforms.

Back-end services such as authorization or data consolidation are also exposed over REST APIs, primarily for back-end to back-end integration.

## How do I get started?

Getting started with the Sinch Verification API and SDK is simple thanks to the extensive documentation for each platform and the different tutorials and sample application available together with the SDKs.

In most cases, Sinch can be used without needing a back-end or any configuration just follow these steps.

1.  [create an account](https://portal.sinch.com/#/signup),
2.  [download the SDK](page:downloads)
3.  get started in minutes following one of the user guide below.
[block:html]
{
  "html": "<div class=\"ug-links\">\n  <div class=\"row\">\n    <a href=\"./verification-for-ios\" class=\"col-md-3 ug-link\">\n      <div class=\"ug-title\">\n        <i class=\"fab fa-apple\"></i><span class=\"title\">iOS</span>\n      </div>\n    </a>\n    <a href=\"./verification-for-android\" class=\"col-md-3 ug-link\">\n      <div class=\"ug-title\">\n        <i class=\"fab fa-android\"></i><span class=\"title\">Android</span>\n      </div>\n    </a>\n    <a href=\"./verification-for-javascript\" class=\"col-md-3 ug-link\">\n      <div class=\"ug-title\">\n        <i class=\"fab fa-js\"></i><span class=\"title\">JavaScript</span>\n      </div>\n    </a>\n    <a href=\"./verification-rest-api\" class=\"col-md-3 ug-link\">\n      <div class=\"ug-title\">\n        <i class=\"fa fa-code\"></i><span class=\"title\">REST</span>\n      </div>\n    </a>\n  </div>\n</div>\n\n<style></style>"
}
[/block]
## How should the SDK and REST API be combined?

The SDK and REST API work together to ensure you the highest possible security and a full control over the verification solution. We recommend the following approach to integrate any of the Verification SDK in your apps:

 1.  Use the SDK to initiate verification requests
 2.  Use the Verification Request Event callback to:
  *   authorize a given verification request to be started
  *   control the amount of retries a single user can attempt
  *   control if a given phone number can be associated to multiple accounts
 3.  Let the SDK automatically intercept (Android only) and report flash calls/SMS to the Sinch backend
 4.  Consolidate the final verification status in your backend using the Verification Result Event callback
[block:image]
{
  "images": [
    {
      "image": [
        "https://files.readme.io/eb29e43-verification_flow.png",
        "verification_flow.png",
        646,
        372,
        "#dee6e4"
      ]
    }
  ]
}
[/block]
## Verification results and success rates

Keep track of verification success rates and results in real time through the Sinch Dashboard. For each verification method, get accurate metrics on how your app is performing:

  - Delivery rate: percentage of numbers who could successfully be reached (phone ringing or SMS delivered)
  - Conversion rate: percentage of unique numbers who could successfully be verified

## How does pricing work?

Verification pricing is calculated on a per request basis. A fixed price is charged for each flash call attempted and a SMS price (depending on country and operator) is charged for each SMS verification attempt.

## Need help?

If you have any questions, feel free to check out our help section or contact us.