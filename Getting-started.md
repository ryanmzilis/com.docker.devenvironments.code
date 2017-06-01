If you ended up here you probably want to update or contribute to the Firefox Design System website, very good! This wiki should give you all the necessary instructions in order to run this website locally or create, edit and publish new pages.

First things first! If you don't have this website running locally read the following instructions in order to do so.

If you already have the website locally running and you're a developer you may want to check the [developing page](https://github.com/firefoxux/photon/wiki/Developing). If you are a content creator you may want to check the [writing page](https://github.com/firefoxux/photon/wiki/Writing). If you are both, check both! As a last step check the [contributing page](https://github.com/firefoxux/photon/wiki/Contributing).

## Install Node.js

Open Terminal.app and check if Node is already installed on your machine:

```bash
$ node -v
```

If Node is not installed you can install it with Homebrew:

```bash
$ brew install node
```

Or, if you don't use Homebrew you can download it from [nodejs.org](http://nodejs.org/download/).

## Clone the repository

If you are part of the Firefox Design System team simply clone the repository. You can do it with Terminal.app or via the [GitHub Desktop](https://desktop.github.com/) app. Once you have downloaded and installed the app go to the repository online on GitHub website and select first _Clone_ and then _Open in Desktop_. For further help check their [guide](https://help.github.com/desktop/guides/contributing/cloning-a-repository-from-github-to-github-desktop/). If you prefer to clone it with Terminal.app run:

```bash
$ git clone git@github.com:firefoxux/photon.git
```

If you are an external contributor first fork the repository and then clone it from your GitHub account.

After you cloned the repository path to the its folder and install all node dependencies with Terminal.app:

```bash
$ cd path/to/repository
$ npm install
```

## `npm` commands

To run (with hot-reloading!):

```bash
$ npm run serve
```

You can now got to [http://localhost:3000](http://localhost:3000) to see the website.

To build:

```bash
$ npm run build
```


