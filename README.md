# [Foundation for Sites](http://foundation.zurb.com) (v6.1)

Foundation is the most advanced responsive front-end framework in the world. Quickly go from prototype to production, building sites or apps that work on any kind of device with Foundation. Includes layout constructs, like a fully customizable, responsive grid, commonly used JavaScript plugins, and full A11Y support.

## Requirements

Requires NodeJS to be installed on your machine. Works with 0.10, 0.12, and 4.1! **Note that parts of our build process will break with NPM 3, due to the changes in how packages are installed.**

The Sass is compiled using libsass, which requires the GCC to be installed on your machine. Windows users can install it through [MinGW](http://www.mingw.org/), and Mac users can install it through the [Xcode Command-line Tools](http://osxdaily.com/2014/02/12/install-command-line-tools-mac-os-x/).

## Setup

### New Project

We recommend using https://github.com/ucla/foundation-zurb-template for static sites and application prototypes.

### Existing Project

To get going with UCLA Branded Foundation in an existing project, run the following command in a directory/folder of your choice.

`git submodule add https://github.com/ucla/foundation-sites.git /`

Which will create a .gitmodules file containing

```
[submodule "foundation-sites"]
	path = /
	url = https://github.com/ucla/foundation-sites.git
```

#### Update

Once installed you can pull down the latest version inside your application by running

`git submodule update --remote foundation-sites`

h3. Further Reading

[Git Tools, Submodules](http://www.git-scm.com/book/en/v2/Git-Tools-Submodules)

## Documentation

Foundation uses [Gulp](http://gulpjs.com/) and [SuperCollider](https://www.npmjs.com/package/supercollider) to generate its [documentation pages](http://foundation.zurb.com/sites/docs). Documentation can also be run from your local computer:

### View documentation locally

You'll want to clone the Foundation repo first and install all the dependencies. You can do this using the following commands:

```
git clone git@github.com:ucla/foundation-sites.git
cd foundation-sites
npm install
```

Then just run `npm start` and the documentation will be compiled. It will also launch an instance of [BrowserSync](http://www.browsersync.io/) and open a tab in your default browser.
The file structure:

```
foundation/
├── dist/
│   └── ...
├── docs/
│   └── ...
```

Copyright (c) 2015 ZURB, inc.
