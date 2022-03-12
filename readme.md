# Vercel Redirect

It's common to run different websites and applications on subdomains. While Vercel supports this in some use cases they unfortunatly don't have frictionless support for all. When you need to use an apex domain (`example.com`) on your Super site and subdomains on other Vercel projects this repository comes in handy. Using this repo you can keep the apex domain on your Vercel account while using a subdomain on Super. The `vercel.json` file is configured to redirect all traffic to `www.example.com`. Here's how you can use this:

1. Clone this repo
2. Replace all instances of `www.example.com` with the `www` subdomain of your domain
3. Deploy a new project in Vercel using your cloned and updated version of this repo
4. Connect your apex domain to that project
5. Add the `www` subdomain to your Super site
6. At this stage an email from Vercel may get send to you asking to give Super access to your `www` subdomain. You'll need to approve this
7. Done! All requests to your apex domain will be redirected to the `www` subdomain you have hosted on Super

[super.so](https://super.so)