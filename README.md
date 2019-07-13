## SuiteCRM Theme for HAR


### Setup

1. Create a new custom theme directory ([custom/themes/SuiteP/](https://github.com/riandesign/har_crm/tree/master/custom/themes/SuiteP))
2. Add new label in a couple of places ([this file](custom/modules/Users/language/en_us.lang.php))
3. Add a new `$app_strings` for the new Theme ([this file](https://github.com/riandesign/har_crm/blob/master/custom/Extension/application/Ext/Language/en_us.NoonThemeLabel.php))
4. Include all custom files ([these files](https://github.com/riandesign/har_crm/tree/master/themes/SuiteP/css/HAR))
5. Finally, just do a **Quick Repair and Rebuild** at [*Admin > Repair > Quick Repair and Rebuild*](http://localhost/har/har_crm/index.php?module=Administration&action=Upgrade), and the *HAR theme* is operational and can be selected from the User’s profile, under Layout options.


### Customizing the styles

In case it's needed to update/customize the style, all you need to do is to custom ([this file](https://github.com/riandesign/har_crm/blob/master/themes/SuiteP/css/HAR/style_har.scss).)

After you change the style file, it's needed to compile it (read topic below).



### Compiling the styles

In order to be able to compile the CSS file, you need to run a SASS compiler and compile only the file **main.scss**. For instance:

`sass --watch main.scss:main.css`



### Tutorial

I followed this [tutorial](https://docs.suitecrm.com/blog/customizing-subthemes/) for creating the custom theme.
