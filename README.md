# Stylelint Installation & Configuration

### Step 1: Open the VS Code (v1.41.1) and search the extension

**stylelint** (current version 0.51.0, thibaudcolas.stylelint) 

### Step 2: Install below Plugins from NPM

**[Stylelint](https://www.npmjs.com/package/stylelint)** or use directly on CLI: **npm i stylelint**

### Step 3 & 4: SCSS users follow the below steps:

**[stylelint-scss](https://www.npmjs.com/package/stylelint-scss)** or use directly on CLI: **npm i stylelint-scss**

**[stylelint-config-sass-guidelines](https://www.npmjs.com/package/stylelint-config-sass-guidelines)** or use directly on CLI: npm i stylelint-config-sass-guidelines

### Step 5: After completed above steps open your project in the VS CODE and follow as below:
Add the **[.stylelintrc.json](https://github.com/suyogn/Stylelint-Configuration/blob/master/.stylelintrc.json)** on the root path in the your project (similar location of package.json)

Download the **[.stylelintrc.json](https://github.com/suyogn/Stylelint-Configuration/blob/master/.stylelintrc.json)**

**Note**: Stylelint has recommended stylelint-config-recommended-scss but needs to install additional plugin as stylelint-order. 
Hence, we choose stylelint-config-sass-guidelines plugin to avoid additional plugin and both plugin almost similar.
**_[stylelint-config-recommended-scss]_**https://www.npmjs.com/package/stylelint-config-recommended-scss 
**_[stylelint-order]_**https://www.npmjs.com/package/stylelint-config-recommended-scss 


# Stylelint rule uses and description:
* "at-rule-name-case": "lower"
> It's prevent to use UPPERCASE/Titlecase as like @Media, @Charset, @MEDIA etc.

* "property-case": "lower"
> The patterns are considered violations WIDTH: 1px; Width: 1px; etc.

* "max-nesting-depth": 3
> Maximum allowing nesting depth 3

  a {

    b { /* 1 */
  
      .foo {} /* 2 */
    
    }
  
  }

* "scss/at-extend-no-missing-placeholder": null
> We can use the placeholder '.' or '%'. Default placeholder is allowed only "%"



