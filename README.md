# My Website

This is a Wowchemy Academic site. The theme module requires Hugo Extended 0.78.2 or newer. On this Mac, run it with **Hugo Extended 0.81.0**. It is not compatible with the latest Hugo installed on the system.

Local server: [http://127.0.0.1:1313/](http://127.0.0.1:1313/)

## Run

The `website-hugo` conda environment contains Hugo Extended 0.81.0, Go, and Git. Do not use the system `hugo`, `go`, or `git`.

```bash
conda activate website-hugo
hugo server --disableFastRender --bind 127.0.0.1 --port 1313
```

## Recreate the environment

conda-forge has no Apple Silicon build of this Hugo version. Install Go and Git with conda, then download the Hugo binary from the release.

```bash
conda create -n website-hugo -c conda-forge go git -y
conda activate website-hugo

curl -fL -o /tmp/hugo.tar.gz \
  https://github.com/gohugoio/hugo/releases/download/v0.81.0/hugo_extended_0.81.0_macOS-ARM64.tar.gz
tar -xzf /tmp/hugo.tar.gz -C /tmp hugo
cp /tmp/hugo "$CONDA_PREFIX/bin/hugo"
chmod +x "$CONDA_PREFIX/bin/hugo"

hugo version
```

`hugo version` should report `v0.81.0` and `extended`.

## Compile and push

Two repositories are involved. This folder is the source (`syoi92/my-wowchemy-site`). `public/` is a separate Git checkout of the GitHub Pages site (`syoi92/syoi92.github.io`). Build into `public/`, push that site first, then push the source so the recorded `public` commit exists on GitHub.

```bash
conda activate website-hugo

# Build the site into public/
hugo --gc --minify
```

Hugo does not delete files it no longer generates. If you removed a photo or video from `content/`, delete the old copy under `public/` before committing. Leftover files stay on the live site, and large ones can make the GitHub Pages deploy time out.

```bash
# 1. Publish the compiled site
cd public
git add -A
git status
git commit -m "Update site"
git push origin master
cd ..

# 2. Publish the source, including the new public commit
git add -A
git status
git commit -m "Update site content"
git push origin master
```

Keep the remotes as they are. The source `origin` is `git@github.com:syoi92/my-wowchemy-site.git`. The `public` `origin` is `git@github.com:syoi92/syoi92.github.io.git`. Do not point the source remote at the Pages repository, and do not pull the source from it.
