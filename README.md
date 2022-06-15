# [Shrey's Resume](resume.shreyc.me)

### How to use

1. Go to [Reactive Resume](https://rxresu.me) and make an account (or [self-host](https://hub.docker.com/r/amruthpillai/reactive-resume) it) 
2. Populate fields with resume data
3. If editing, download .json file from this repo and upload to resume builder before editing
4. Download .json and .pdf files when done
5. Push both files to this git repo (version control)
6. Github actions should automatically generate a page at https://sxc97.github.io/resume/ with the pdf embedded
7. If not, go to settings -> pages, select the main branch and the root directory as the source before clicking save. Once you select a theme, the site should go live.

### Custom domain name

1. Buy domain name (I used Hover)
2. Set up Cloudflare account
3. Create new A Record with your subdomain (in this case "resume") and set the IPv4 address to 8.8.8.8
4. Go to page rules and set up a 301 redirect from the subdomain to the github page (e.g. resume.shreyc.me -> https://sxc97.github.io/resume/)
