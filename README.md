# CogDyn Lab Quarto Website Starter

This is a starter Quarto website for `https://cogdynlab.org`.

## Recommended repository

Create a GitHub organization named `cogdynlab` and a repository named:

```text
cogdynlab.github.io
```

This makes the default GitHub Pages domain `https://cogdynlab.github.io`, which is convenient for DNS records.

If you use a different GitHub organization or username, update:

- `_quarto.yml` GitHub link
- DNS CNAME target for `www.cogdynlab.org`

## Local preview

Install Quarto, then run:

```bash
quarto preview
```

## Render locally

```bash
quarto render
```

The rendered site will be generated in `_site/`.

## GitHub Pages deployment

1. Push this folder to the `main` branch of your GitHub repository.
2. In GitHub, go to **Settings > Pages**.
3. Set **Build and deployment > Source** to **GitHub Actions**.
4. Push to `main` again or run the workflow manually from the **Actions** tab.
5. After the first deployment, add custom domain `cogdynlab.org` in **Settings > Pages**.
6. Configure DNS at your domain registrar.

## DNS records

For the apex domain `cogdynlab.org`, create these A records:

```text
@  A  185.199.108.153
@  A  185.199.109.153
@  A  185.199.110.153
@  A  185.199.111.153
```

Optional IPv6 AAAA records:

```text
@  AAAA  2606:50c0:8000::153
@  AAAA  2606:50c0:8001::153
@  AAAA  2606:50c0:8002::153
@  AAAA  2606:50c0:8003::153
```

For `www.cogdynlab.org`, create:

```text
www  CNAME  cogdynlab.github.io
```

If your GitHub organization/username is not `cogdynlab`, replace the target with `<your-org-or-username>.github.io`.

## Files to edit first

- `index.qmd` — lab intro and main research themes
- `people.qmd` — PI, students, alumni
- `publications.bib` — real publications
- `join.qmd` — recruitment details
- `contact.qmd` — email, address, map links
- `_quarto.yml` — navigation, site title, GitHub link

## Custom domain file

The `CNAME` file contains:

```text
cogdynlab.org
```

Keep this file in the project root so Quarto includes it in the rendered site.
