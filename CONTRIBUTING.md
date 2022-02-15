# CONTRIBUTING

- [CONTRIBUTING](#contributing)
    - [Build locally](#build-locally)
        - [Prerequisites](#prerequisites)
            - [node.js](#nodejs)
            - [Hugo](#hugo)
        - [Clone repo and its submodules](#clone-repo-and-its-submodules)
        - [Install javascripts dependencies](#install-javascripts-dependencies)
        - [Serve the website locally](#serve-the-website-locally)

## Build locally

### Prerequisites

#### node.js

A quick version (for Mac and Linux) that will also allow to manage different version of node
is to install node via the "node version manager".

```bash
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
```

open a new terminal or source your .bashrc and then:
```bash
nvm install node
```

#### Hugo

- [See the install page](https://gohugo.io/getting-started/installing/)

one example for Linux or for the [Windows Sub-system for Linux](https://docs.microsoft.com/en-us/windows/wsl/install):
```bash
wget https://github.com/gohugoio/hugo/releases/download/v0.92.2/hugo_extended_0.92.2_Linux-64bit.tar.gz
tar xfz hugo_extended_0.92.2_Linux-64bit.tar.gz
echo "export PATH=`pwd`:\$PATH" >> ~/.bashrc
source ~/.bashrc
which hugo
```

### Clone repo and its submodules

```
git clone --recurse-submodules https://github.com/brainhackorg/brainhack_cloud
cd brainhack_cloud
```

If you have only cloned the repo and did not get all the submodules (`docsy` and `docsy`'s own subdmodules),
simply run

```
git submodule update --init --recursive && git submodule update --recursive
```

### Install javascripts dependencies

```
npm install
```

### Serve the website locally
```
hugo server -D
```
