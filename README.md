# Telefónica theme for Twitter Bootstrap 3

Telefónica Corporative Bootstrap Theme for easy and quick web page prototyping.

See it live at https://telefonica.github.io/TEFstrap

## Quick start

Several quick start options are available:

* [Download the latest release](https://github.com/Telefonica/TEFstrap/releases)
* Clone the repo: `git clone https://github.com/Telefonica/TEFstrap.git`
* Install with [Bower](http://bower.io): `bower install tefstrap`
* Install with [npm](https://www.npmjs.com): `npm install @telefonica/tefstrap`

Here you get the most basic form of TEFstrap: precompiled files for quick drop-in usage in nearly any web project. Just replace your original `bootstrap.css` with the TEFstrap one you downloaded, located at `dist/css/bootstrap.css` and copy the fonts `dist/fonts/` directory to your own one. 

## Hacking

After downloading the proyect, you can modify and compile your own distributon with your own customizations, or just pick some parts. 
The pre-compiled `bootstrap.css` distributed in `dist/` directory is precompiled and minified, and  
the `less/`, `js/`, and `fonts/` are the source code for our CSS, JS, and fonts (respectively). 

Three source files are provided in the `less` directory:
* `less/tefstrap`: Custom components and variables for TEfstrap
* `less/variables.less`: A copy of bootstrap variables, but with the values for the Telefonica theme.
* `less/bootstrap.less`: The main entry point for compile TEFstrap. Loads all bootstrap and applies the TEFstrap customizations. Here you can be quirurgic: make your own and just import your desired bootstap files, add the above two files and then compile it

Both boostrap and tefstrap does not add proactively all the browser vendor prefixes. Therefore you will need to use the [`autoprefixer`](https://github.com/postcss/autoprefixer) tool. 

Finally take a look to our `package.json#scripts.build` for inspiration about how to compile/autoprefix/minify less files and generate the CSS ones

## Development

First of all, [download and install NodeJS](https://nodejs.org).

```sh
git clone https://github.com/Telefonica/TEFstrap.git
cd TEFstrap
npm install # Install node dependencies for this project
npm run build # Build (i.e compile/autoprefix/minify) assets
npm run dev # Start development watchers, to auto compile less
open index.html # Open the index.html with your default browser
```

# LICENSE

Copyright (c) 2011-2016 [Telefónica I+D](https://tid.es). Code released under the [MIT license](LICENSE). 

[Bootstrap](https://github.com/twbs/bootstrap): copyright 2011-2016 Twitter, Inc. Code released under the [MIT license](https://github.com/twbs/bootstrap/blob/master/LICENSE).

