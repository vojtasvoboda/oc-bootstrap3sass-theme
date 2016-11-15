Bootstrap 3 Sass
================

Bootstrap 3 theme for OctoberCMS with [Sass](http://sass-lang.com/) support.

- Why another Bootstrap theme? -- This theme is prepared with Sass preprocessor.
- Why [Bootstrap 3](http://getbootstrap.com/) and not Bootstrap 4? -- Because v3 is last stable and v4 is only alpha version.

## Features

- build on the top of official **stable library** by Twitter
- ready made with the [Sass](http://sass-lang.com/) with **no need to compiling**
- dependencies managed by **[Yarn](https://yarnpkg.com/) and [Bower](https://bower.io/)** with easy updating
- [FontAwesome](http://fontawesome.io/) and [Font Lato](http://www.latofonts.com/lato-free-fonts/) included
- prepared theme configuration file, just add your own fields

## Local development

For local development be sure, that you have `cms.enableAssetDeepHashing` config set to `true`!

## Configure Bootstrap

Sass main file is placed at `/assets/sass/site.scss`. All Sass files you want to use should be imported here.

All Bootstrap Sass components are imported at `/assets/sass/_settings.scss` - just uncommend component you need. Always use only component you really need to make your CSS smaller and your sites faster.

All Bootstrap JS components are linked at the bottom of layout `/layouts/default.htm`. Just comment lines you don't need.

At `/assets/sass/_settings.scss` you can find all Bootstrap configuration variables which you can change and also add your own variables to the top of the file. It will override default Bootstrap variables, so it's mean then you always compile customized version of Bootstrap.

## Theme variables

Theme variables are placed at `/fields.yaml` file. Just add your own variables and use it in theme:

```
{{ this.theme.site_title }}
```

Then set this variables at Backend > CMS > Themes > Customize.

## Add new font

- place your font to `/assets/fonts` directory
- create new Sass file at `/assets/sass/fonts`
- import this font Sass file to `/assets/sass/site.scss` like this:

```
@import "fonts/font-awesome";
```

## Updating

You can update theme dependencies by yourself, but it's not neccesary.

- update npm by `yarn update` or `npm update`
- update assets by `bower update`

## About

Bootstrap 3 Sass theme is made with [bootstrap-sass](https://github.com/twbs/bootstrap-sass) library, which is official Sass port of Bootstrap 3 framework by Twitter.

## Contributing

**Feel free to send pullrequest!** Please send pull request to master branch.

## Todo

- [ ] Install FontAwesome by Bower.

## Copyright and License

Theme released under the [MIT](https://github.com/vojtasvoboda/oc-bootstrap3sass-theme/blob/master/LICENSE) license.
