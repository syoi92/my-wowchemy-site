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
