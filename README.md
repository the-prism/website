## Configure dev environment

> Instructions are for Linux / windows 10 bash

Make sure Linux is up to date.

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
sudo gem install jekyll
```

In order to run the website locally you can either use vs code with the tasks already setup, or simply run `jekyll serve` in the folder.

# Bootstrap

Bootstrap is used for the css in it's uncompiled sass format in the css folder. Compilation is configured in the `_config.yml` file. The current version of the source files is `4.0` Future update may be required for patches.

> Tutorials and components are described in the documentation. [More info here](https://getbootstrap.com/docs/4.0/getting-started/introduction/)
