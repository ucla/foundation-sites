# [Foundation for Sites - Forked](http://foundation.zurb.com)

## Requirements

Requires NodeJS to be installed on your machine. Works with version 4 and higher!

The Sass is compiled using libsass, which requires the GCC to be installed on your machine. Windows users can install it through [MinGW](http://www.mingw.org/), and Mac users can install it through the [Xcode Command-line Tools](http://osxdaily.com/2014/02/12/install-command-line-tools-mac-os-x/).

## Setup

### New Project

We recommend using https://github.com/ucla/foundation-zurb-template for static sites and application prototypes.

### Existing Project

To get going with UCLA Branded Foundation in an existing project, run the following command in a directory/folder of your choice.

`git submodule add -b develop -f https://github.com/ucla/foundation-sites.git bower_components/foundation-sites`

Which will create a .gitmodules file containing

```
[submodule "bower_components/foundation-sites"]
	path = bower_components/foundation-sites
	url = https://github.com/ucla/foundation-sites.git
	branch = develop
```

Then run `npm start` to compile the documentation. When it finishes, a new browser window will open pointing to a BrowserSync server displaying the documentation.

## Testing

Foundation has three kinds of tests: JavaScript, Sass, and visual regression. Refer to our [testing guide](https://github.com/zurb/foundation-sites/wiki/Testing-Guide) for more details.

These commands will run the various tests:

- `npm run test:sass`
- `npm run test:javascript`
- `npm run test:visual`

## Update

Once installed you can pull down the latest version inside your application by running

`git submodule update --remote foundation-sites`

### Further Reading

[Git Tools, Submodules](http://www.git-scm.com/book/en/v2/Git-Tools-Submodules)

## Documentation

Foundation uses [Gulp](http://gulpjs.com/) and [SuperCollider](https://www.npmjs.com/package/supercollider) to generate its [documentation pages](http://foundation.zurb.com/sites/docs). Documentation can also be run from your local computer.

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
