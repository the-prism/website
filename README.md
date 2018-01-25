## Configure dev environnement

> Instructions are for linux / windows 10 bash

Make sure linux is up to date.

```bash
sudo apt update
sudo apt upgrade
```

Install ruby is it's not installed yet.

```bash
sudo apt-add-repository ppa:brightbox/ruby-ng
sudo apt-get update
sudo apt-get install ruby2.3 ruby2.3-dev build-essential
```

After that we need to install all the gems required.

```bash
sudo gem update
sudo gem install jekyll bundler
```

Before installing the github-pages gem we need some unlisted libraries required to build the dependencies.

```bash
sudo apt install libxslt-dev libxml2-dev zlib1g-dev
```

Then we can install the last required gem. *Note,* this will take a while.

```bash
sudo gem install github-pages
```

# Bootstrap

Bootstrap is used for the css in it's uncompiled sass format in the css folder. Compilation is configured in the `_config.yml` file. The current version of the source files is `4.0` Future update may be required for patches.

> Tutorials and components are described in the documentation. [More info here](https://getbootstrap.com/docs/4.0/getting-started/introduction/)
