# [Shrey's Resume](resume.shreyc.me)

### How to generate resume (Optional)

1. Go to [Reactive Resume](https://rxresu.me) and make an account (or [self-host](https://hub.docker.com/r/amruthpillai/reactive-resume) it) 
2. Populate fields with resume data
3. If editing, download .json file from this repo and upload to resume builder before editing
4. Download .json and .pdf files when done
5. Push both files to this git repo (version control)

### How to set up Github Pages
1. Add new file in root directory called `index.html`
2. Paste the following code
```
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
 <html lang="en" style="width:100%; height:100%;">
 <head>
   <meta http-equiv="content-type" content="text/html; charset=utf-8">
   <title>Shrey's Resume</title>
 </head>
   <body style="width:100%; height:100%; margin:0;">
<iframe src="https://docs.google.com/viewerng/viewer?url=https://github.com/SxC97/resume/raw/main/SHREY_CHOUDHARY_RESUME.pdf&embedded=true" frameborder="0" height="100%" width="100%">
</iframe>
  </body>
 </html>
```
3. On line 3:

```
<iframe src="https://docs.google.com/viewerng/viewer?url=https://github.com/SxC97/resume/raw/main/SHREY_CHOUDHARY_RESUME.pdf&embedded=true" frameborder="0" height="100%" width="100%">
```

the url is to the google docs pdf viewer. This is used incase the browser doesn't have a built in pdf viewer.

4. The link in the middle (`url=`) should be directed to the resume.pdf file you uploaded previously. Click on the pdf document, then right click on the download button and copy the link address.
5. Note: If you upload a pdf with a different file name, you will have to change the link here.
6. After saving, Github Actions should automatically generate a page at https://sxc97.github.io/resume/ with the pdf embedded
7. If not, go to settings -> pages, select the main branch and the root directory as the source before clicking save. Once you select a theme, the site should go live.

### Custom domain name (Optional)

1. Buy domain name (I used Hover)
2. Set up Cloudflare account
3. Create new `A Record` with your subdomain (in this case "resume") and set the IPv4 address to `8.8.8.8`
4. Go to page rules and set up a 301 redirect from the subdomain to the github page (e.g. `resume.shreyc.me -> https://sxc97.github.io/resume/`)
