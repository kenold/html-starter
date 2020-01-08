## Instructions
You need to install Node JS to run `npm` commands. So, verify that Node.js is installed first. To check if Node JS is installed on your computer, run `which npm` in a terminal. If you see a `/nodejs/npm` path, you have Node JS - if not, follow the instructions at [nodejs.org](https://nodejs.org/en/) to install.

1. Install the packages from package.json: `npm install`
2. Install live-server package globally (-g): `npm install -g live-server`
3. Run `npm start` to start live server

When you save `main.scss` (/sass/main.scss), a file named `style.css` will be created in `assets/css`. Do not edit `style.css`; work with `main.scss` instead.

## Font
The starter is using the ***Inter*** font. More info at [https://rsms.me/inter/](https://rsms.me/inter/). The font is located in the fonts partial at sass/_fonts.scss. Optional local font files area also included (assets/fonts) if you'd like to work offline.

## Mixins
#### Breakpoints (Responsive)
Use the breakpoint mixin as follow:
`
h1 {
    margin-top: 12px;
    @include md {
        margin-top: 20px;
    }
}
`

#### Font Size
The font size mixin convert px unit to rem unit. The default size is 16px (or 1rem).
h1 {
    @include font-size(18);
}

will exand to:
`
h1 {
    font-size: 1.125rem;
}
`

#### Centering

Created by [Kenold Beauplan](https://twitter.com/kenoldb)
