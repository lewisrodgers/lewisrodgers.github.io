---
layout: post
title: "Mapping a custom domain to your App Maker app"
description: "An App Maker deployment URL is long and gross. Learn how to create a short memorable URL instead."
date: 2019-09-03 00:00:00 -0400
tags: [G Suite]
image: "assets/posts/2019-09-03/featured.png"
image-alt: "Illusration of the App Maker logo next to a faux custom domain."
---
While it’s possible to map a friendlier URL to an App Maker deployment, it requires privileged access to your domain registrar or organization’s G Suite admin console. If you don’t have this level of clearance, then you’ll need to coordinate with your organization's admins to do some of the things described below.

## Subdomain forwarding

A unique URL is created when deploying an App Maker application and looks something like this:

```
https://script.google.com/a/macros/company.com/s/AKfyc.../exec
```

If you manage a domain, a shorter and more readable URL can be configured with subdomain forwarding. The steps to do this depends on the domain registrar (e.g., Google Domains, Bluehost, etc.).

{% include image.html name="subdomain-forwarding.png" caption="Domain forwarding in Google Domains." %}

So imagine creating a catchy subdomain like `coolfinancecalculator.company.com` and mapping it to your not-so-short App Maker app URL.

## G Suite web address mapping

As a G Suite administrator, you can assign (map) a URL to a site in Google Sites. Instead of the default sites.google.com/a/yourdomain.com/yoursitename, you can create shorter, easy-to-remember addresses for your public websites (like company.com/productname). You can create up to 2000 custom site addresses with your G Suite account.[^1]

{% include image.html name="add-a-new-web-address-mapping.png"%}

Once you’ve created the Google Site, embed (or add a link to) the deployed App Maker application.

{% include image.html name="embedded-app-maker.png" caption="App Maker app embedded on a Google Site." %}

Think about using a Google Site as a landing page for multiple related App Maker applications. And maybe even store documentation on how to use these apps here, too.

## Custom deployment URL

There’s an [open feature request](https://issuetracker.google.com/issues/63382989){:target="_blank"} in the Google issue tracker (opened in 2017) requesting the ability to customize the deployment URL to improve readability. This would be a nice alternative since any App Maker author could customize the deployment URL directly from the App Maker UI. But, it's hard to say when, or if, this feature will become available. 


[^1]: [https://support.google.com/a/answer/7392423](https://support.google.com/a/answer/7392423){:target="_blank"}
