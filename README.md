# Shrey's Resume

### How to use

1. Go to [Reactive Resume](https://rxresu.me) (or self-host it) and populate fields with resume data
2. If editing, download .json file from this repo and upload to resume builder
3. Download .json and .pdf files when done
4. Push both files to this git repo (version control)
5. Github actions should automatically generate a page at https://sxc97.github.io/resume/ with the pdf embedded

### Custom domain name

1. Buy domain name (I used Hover)
2. Set up Cloudflare account
3. Create new A Record with your subdomain (in this case "resume") and set the IPv4 address to 8.8.8.8
4. Go to page rules and set up a 301 redirect from the subdomain to the github page (e.g. resume.shreyc.me -> https://sxc97.github.io/resume/)
