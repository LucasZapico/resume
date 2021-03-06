# Resume

Resume of Kazuya Gosho, built with Webpack + Pug + Postcss.

![screenshot](https://github.com/acro5piano/resume/blob/master/screenshot.en.png)

# Getting started

After checking out the repo, run:

```
yarn install
yarn start
```

open localhost:3000 and you can see my resume.

# Write your resume with this template

Feel free to write your resume with this template, if you are enough odd to do so.

- `src/app.postcss` is for css
- `src/index.pug` is for template
- If you want to write your resume with sass, just add `sass-loader`

# Internationalization

Unfortunatelly, we only have really legacy option to this setting.

To create Japanese resume, `HtmlWebpackPlugin` in `webpack.config.js` like this:

```
  plugins: [
    new HtmlWebpackPlugin(
      {
        template: './index.ja.pug',
        filename: 'index.html',
        inject: false
      }
    )
  ]
```

# Screenshot

To take a screenshot, just run

- `yarn start`
- `yarn screenshot`

This runs your Chrome headlessly and take an image.

# TODO

- [x] Add script for taking screenshot.
- [ ] Add ESLint for stability.
- [ ] Add Flow for type-safe and null-safe.
- [ ] Internationalization. currently I need `en` and `ja`. For the time being create `index.ja.pug`.
- [ ] Use React.js or Vue.js for template. This is for HMR and scoped CSS and internationalization.
- [ ] Add script for build. Generate multilingual PDF to `/dist`.
- [ ] `screenshot` command Internationalization.
- [ ] Create GitHub page or something to render this as actual web page.
  - [ ] Hopefully, change language interactively.

# Contribution

I am not a native English speaker, so if you find something wrong, please create an issue or send a pr.

Thanks in advance.
