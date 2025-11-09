
MavenStrides Static Site - Multi-page site for Netlify deployment
---------------------------------------------------------------

Included files:
- index.html
- services.html
- training.html
- portfolio.html
- about.html
- contact.html
- assets/styles.css

How to push to GitHub and connect to Netlify
-------------------------------------------

1) Create an empty GitHub repository (if you haven't) e.g., mavenstrides-site.
2) On your local machine:
   git clone git@github.com:YOURUSERNAME/REPO.git
   cd REPO
   Copy the unzipped files into this repo, then:
   git add .
   git commit -m "Initial MavenStrides site"
   git push origin main

3) Connect repository to Netlify:
   - Netlify: New site from Git -> GitHub -> select the repo
   - Build command: (leave blank)
   - Publish directory: / (root)
   - Deploy site

4) Alternatively, deploy manually by adding a new site -> Drag & Drop the ZIP contents via "Deploy manually".

Notes on forms and email forwarding
-----------------------------------
- Forms use Netlify Forms (data-netlify="true"). Submissions appear in Netlify dashboard -> Forms.
- To forward submissions to info@ and booking@, you'll need to configure an integration:
  Option A: Use Netlify's built-in notifications (webhook) to forward to a service (n8n, Zapier).
  Option B: Use a small serverless function to relay emails.
I can help wire the automation (n8n flow) after you connect the repo to Netlify.
