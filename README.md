# Stylelint Installation & Configuration

## Step 1: Open the VS Code and search the extension

**_stylelint_**

thibaudcolas.stylelint (It's extension identifier current version 0.51.0)

## Step 2: Install below Plugins from NPM

2. **_[Stylelint]_**https://www.npmjs.com/package/stylelint
...You can use directly on CLI: npm i stylelint

## If you're working with SCSS then follow the below steps:

3. **_[stylelint-scss]_**https://www.npmjs.com/package/stylelint-scss
...You can use directly on CLI: npm i stylelint-scss

4. **_[stylelint-config-sass-guidelines]_**https://www.npmjs.com/package/stylelint-config-sass-guidelines
...You can use directly on CLI: npm i stylelint-config-sass-guidelines

## Once the complete above steps then open your project in the VS CODE and follow as below:
5. Download the .stylelintrc.json from here and paste in your project on root path (similar location of package.json)

Note: Stylelint has recommended stylelint-config-recommended-scss but needs to install additional plugin as stylelint-order. 
Hence, we choose stylelint-config-sass-guidelines plugin to avoid additional plugin and both plugin almost similar.
**_[stylelint-config-recommended-scss]_**https://www.npmjs.com/package/stylelint-config-recommended-scss 
**_[stylelint-order]_**https://www.npmjs.com/package/stylelint-config-recommended-scss 


# Stylelint rule uses and description:
..* "at-rule-name-case": "lower"
...It's prevent to use UPPERCASE/Titlecase as like @Media, @Charset, @MEDIA etc.

..* "property-case": "lower"
...The patterns are considered violations WIDTH: 1px; Width: 1px; etc.

..* "max-nesting-depth": 3
...Maximum allowing nesting depth 3
...a {
... b { /* 1 */
...   .foo {} /* 2 */
... }
...}

..* "scss/at-extend-no-missing-placeholder": null
...We can use the placeholder '.' or '%'. Default placeholder is allowed only "%"



