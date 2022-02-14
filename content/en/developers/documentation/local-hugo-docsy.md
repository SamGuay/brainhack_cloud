---
title: "Local Hugo Docsy"
linkTitle: "Local Hugo Docsy"
weight: 1
description: >
  How to edit the documentation
---

## Local Hugo Docsy

### Clone repository
Using SSH

`git clone --recurse-submodules git@github.com:NeuroDesk/neurodesk.github.io.git`

or Https:

`git clone --recurse-submodules https://github.com/NeuroDesk/neurodesk.github.io.git`

### If you cloned without --recurse-submodules

Run the following command to pull submodules

`git submodule update --init --recursive --remote`

### Download Hugo binary

Hugo releases are on https://github.com/gohugoio/hugo/releases

Download latest version of hugo extended

e.g. for windows: https://github.com/gohugoio/hugo/releases/download/v0.88.1/hugo_extended_0.88.1_Windows-64bit.zip


### Start local hugo server

Extract hugo binary (hugo.exe) to your neurodesk.github.io dir

Run server for windows: `.\hugo.exe server --disableFastRender`

Once started, dev website will be accessible via http://localhost:1313

### Update docsy theme submodule
<pre class="language-shell command-line" data-prompt="$"><code>git submodule update --remote
git add themes/
git commit -m "Updating theme submodule"
git push origin hugo-docsy</code></pre>
