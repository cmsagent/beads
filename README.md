# Our Bead Shop

Static bead shop website intended for https://beads.stevensnetwork.co.uk/.

## Site files

- `index.html` — website page
- `assets/` — original craft photographs, cropped and rotated for display

No build step or dependencies are required. Publish `index.html` and `assets/` to the web root of the hosting destination. Asset paths are relative and work at the subdomain root.

## AWS deployment

The GitHub repository alone does not deploy the website. Connect the `main` branch to your AWS deployment, or upload the site files to the S3 origin for the subdomain's CloudFront distribution. Set `index.html` as the default root object. The CloudFront distribution needs the `beads.stevensnetwork.co.uk` alternate domain name and a matching TLS certificate; DNS must point the subdomain to that distribution.

This repository contains no AWS credentials or deployment workflow. Configure the AWS destination and GitHub deployment authentication before enabling automatic deployment.
