# bf-premeng-pwa-language-packs

This package provides language packs beyond the `en_US.json` provided in
venia-ui.

## Installation

This pack is already installed, but how it was installed, for information:
To install this pack, just add it as devDependency to `bf-premend-ecommerce-frontend` or your
project:

Example:

`yarn add "@bigfishgames-opensource/bf-premeng-pwa-language-packs"@git+https://github.com/bigfishgames-opensource/bf-premeng-pwa-language-packs#1.0.3 -D`

## Local Development

Go to the [Language Pack Github](https://github.com/bigfishgames-opensource/bf-premeng-pwa-language-packs) and checkout the repository.  Place it next to the `bf-premeng-ecommerce-frontend` repository checkout on your machine.

Next change directory into the location of the lanuage packs you just checked out.  `cd ~/Sites/bf-premeng-pwa-language-packs` and run `yarn link`.  You should get output similar to below:

```
success Registered "@bigfishgames-opensource/bf-premeng-pwa-language-packs".
info You can now run yarn link "@bigfishgames-opensource/bf-premeng-pwa-language-packs" in the projects where you want to use this module and it will be used instead.
```

Now change directories back to your frontend application directory.

```
cd ~/Sites/bf-premend-ecommerce-frontend
```

Then link using the command from the output you got when you ran `yarn link` from the package directory. E.g.

```
yarn link "@bigfishgames-opensource/bf-premeng-pwa-language-packs" 
```

To unlink a package that was symlinked during development in your project, simply run:
 ```
 yarn unlink @bigfishgames-opensource/bf-premeng-pwa-language-packs
 yarn install --check-files
 ```