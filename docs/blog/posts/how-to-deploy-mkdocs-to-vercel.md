---
draft: false
date: 2024-04-11
categories:
  - website
  - blog
  - vercel
  - amazon linux
authors:
  - lowikian
---
# Deploying Material for MkDocs to Vercel

Since we are using Vercel for Hosting the Blog to make sure it dosen't go down when our Provider has issues, we thought we'd make a small tutorial on how to Deploy Material for MkDocs to Vercel

We asume you already connected your repo with vercel or set it up some other way.

1. Go to the Vercel Dashboard and go the Build settings
2. Enter the following values

```
Build Command: mkdocs build
Output Directory: site
Install Command: pip install urllib3==1.26.6 && pip install -r requirements.txt
```

When it's done it should something like this
![Image showing our Build settings](/static/build-settings.png)
3. Click on save      
4. Try running `vercel` and if the Build succeeds than you're done!


We hope this helped someone since we had this issue and found nothing online.
