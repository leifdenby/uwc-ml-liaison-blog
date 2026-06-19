# UWC ML Liaison Blog

Quarto website for `UWC ML Liaison Notes`, a public working notebook on
machine-learning weather prediction, verification, physical processes, and
collaboration across UWC.

Editorial planning, launch scope, and content ideas are in
[`content-plan.md`](content-plan.md).

## Local Development

Quarto is required to preview or render the site.

Check whether Quarto is installed:

```sh
quarto --version
```

If that command is not found, install Quarto from:

<https://quarto.org/docs/get-started/>

Start the local development server:

```sh
quarto preview
```

Build the static site:

```sh
quarto render
```

Rendered output is written to `_site/`, as configured in `_quarto.yml`.

## Deployment

The site is deployed to GitHub Pages by `.github/workflows/deploy.yml` whenever
changes are pushed to `main`. The workflow renders the Quarto site and publishes
the `_site/` directory.

The public URL is:

<https://uwc-ml.denby.eu>

The custom domain is configured by the top-level `CNAME` file, which Quarto
copies into the rendered site.

Blog post comments are powered by
[utterances](https://utteranc.es/) using GitHub Issues in this repository. To
enable them, turn on Issues for the repository and install the utterances GitHub
App for `leifdenby/uwc-ml-liaison-blog`.

DNS should contain:

```text
uwc-ml.denby.eu  CNAME  leifdenby.github.io
```

In the GitHub repository settings, configure Pages to use GitHub Actions as the
deployment source and enable HTTPS once DNS validation succeeds.
