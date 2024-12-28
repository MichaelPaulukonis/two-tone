# TWO-TONE

Display two different monochrome images in two different colors.<br>
So, two-hue, not two-tone.<br>
Whatevs.


- inspired by https://bsky.app/profile/leedoughty.bsky.social/post/3ldh2esstd22h
  - https://leedoughty.com/

## TODO: use image.mask

Convert b&w monochromes to black+transparent:

`convert monochrome.png -fuzz 80% -transparent white transparent.png`

Then with `image.mask('foo.png')` it should be WAAAAAAY faster than the pixel stuff

NOTE: ACKSHUALLY it uses pGraphics not image.mask and `pg.drawingContext.globalCompositeOperation = 'source-in'`

see POC @ <https://editor.p5js.org/MichaelPaulukonis/sketches/6gqXLICTo>


## P5.js-vite Starter Template 🚀

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

[Vite](https://vitejs.dev/) starter template to scaffold a new [p5.js](https://p5js.org) project.

This is an unopinionated template; aside from P5.js and Vite, the rest of your project's tools are entirely up to you.

## Live demo

For a live demo please [visit this page](https://p5js-vite-demo.surge.sh).

## Installation

Pull the template files with [degit](https://github.com/Rich-Harris/degit) and install dependencies.

```
npx degit makinteract/p5js-vite my-project

cd my-project
npm install
npm run dev
```

## npm scripts

- `npm run dev` - Starts the development server at port [3000](http://localhost:3000/)
- `npm run build` - Builds the application in a `dist` folder
- `npm run preview` - Serves the build files (`dist` folder) locally at port [5000](http://localhost:3000/)

Note that if after this last command you do not see anything, you can use instead this other command:

- `npm run preview --host` - You should then be able to see your files locally at port [5000](http://localhost:3000/)

## License

This project is open source and available under the [MIT License](LICENSE).
