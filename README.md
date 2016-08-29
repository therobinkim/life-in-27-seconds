# Life Explained in 27 Seconds

## What this?

This is an Electron `.app` bundle that loads Casey Neistat's [Life Explained in 27 Seconds](https://www.youtube.com/watch?v=L9VBpbnXhWk) YouTube movie via [ListenOnRepeat.com](http://listenonrepeat.com/watch/?v=L9VBpbnXhWk#Life_Explained_in_27_Seconds). Basically, you can [download](https://github.com/therobinkim/life-in-27-seconds/archive/master.zip) everything in this GitHub repository to your Mac and run it as a regular desktop app to watch Casey's movie on repeat!

## Why make?

I enjoy having this movie repeat nonstop on my extra monitor. By bundling it into its own app, I can separate it from my regular Chrome browser windows.

## How make?

The `Life Explained in 27 Seconds.app/Contents/Resources/app` [directory](./Life%20Explained%20in%2027%20Seconds.app/Contents/Resources/app) holds my own code. I wrote that code via the [prebuilt quick start app example](http://electron.atom.io/docs/tutorial/quick-start/#try-this-example). (Actually, I just used the quick start example and changed 2 lines of code.)

I then downloaded `electron-v1.3.4-darwin-x64.zip` from https://github.com/electron/electron/releases as per http://electron.atom.io/docs/tutorial/quick-start/#macos.

Afterwards, I followed the tips from http://electron.atom.io/docs/tutorial/application-distribution/ and put my `main.js` and `package.json` files in the `Life Explained in 27 Seconds.app/Contents/Resources/app` [directory](./Life%20Explained%20in%2027%20Seconds.app/Contents/Resources/app) (same one from up above).

I tweaked the names of the helper apps as well. However, renaming `Electron` in the `Life Explained in 27 Seconds.app/Contents/MacOS` [directory](./Life%20Explained%20in%2027%20Seconds.app/Contents/MacOS) to `Life Explained in 27 Seconds` would NOT allow me to open `Life Explained in 27 Seconds.app` any more. So, I left its name as `Electron`.

## What next?

ListenOnRepeat is awesome, but I'd like to see if I can reduce the app's memory usage by creating my own HTML page that only loads the bare minimum YouTube player and nothing else. [#1](https://github.com/therobinkim/life-in-27-seconds/issues/1)

I'd like to be able to change the source code in the in `Life Explained in 27 Seconds.app/Contents/Resources/app/` [directory](https://github.com/therobinkim/life-in-27-seconds/tree/master/Life%20Explained%20in%2027%20Seconds.app/Contents/Resources/app) and have Mac and Windows desktop apps be automatically created/bundled. [#2](https://github.com/therobinkim/life-in-27-seconds/issues/2)

**However, I do not plan on dedicating any additional time to this project, so will happily accept pull requests!** ...and tips for working with Electron, so I don't have to upload a 120.9 MB folder to GitHub.
