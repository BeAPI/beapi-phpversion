<a href="https://beapi.fr">![Be API Github Banner](/assets/banner-github.png)</a>

# BEA PHP Version #

## Description ##

Check current PHP version and optionally compare with your project's requirement.

## Screenshots

![Error displayed in widget at glance](/assets/screen-error-glance.png)
![Error displayed in admin footer text](/assets/screen-error-footer.png)
![php version displayed in widget at glance](/assets/screen-glance.png)
![php version displayed in admin footer text](/assets/screen-footer.png)

## Installation

### WordPress

- Download and install using the built-in WordPress plugin installer or optionnaly, consider using it as mu-plugin
- Site activate in the "Plugins" area of the admin.
- Nothing to do then !

### [Composer](http://composer.rarst.net/)

- Add repository source : `{ "type": "vcs", "url": "https://github.com/BeAPI/bea-phpversion" }`.
- Include `"bea/bea-phpversion": "dev-master"` in your composer file for last master's commits or a tag released.
- Nothing to do then !

## Optional

By default it will only print current php version (tidy format) in the dashboard at glance and in admin footer text but if you add a constant in your wp-config (or dotenv) that defines the php version of your project (php version in production) :

	define( 'BEA_PHP_VERSION', '7.2' );

it will compare the two versions and if it does not match you will be alerted. It's especially useful when dealing with multiple environments.

## Filters

*bea_phpversion_is_allowed* : default is `is_super_admin()` (which allows only administrators on single installations).

## Contributing

Please refer to the [contributing guidelines](.github/CONTRIBUTING.md) to increase the chance of your pull request to be merged and/or receive the best support for your issue.

### Issues & features request / proposal

If you identify any errors or have an idea for improving the plugin, feel free to open an [issue](../../issues/new) or [create a pull request](../../compare). Please provide as much info as needed in order to help us resolving / approve your request.

## Who ?

Created by [Be API](https://beapi.fr), the French WordPress leader agency since 2009. Based in Paris, we are more than 30 people and always [hiring](https://beapi.workable.com) some fun and talented guys. So we will be pleased to work with you.

This plugin is only maintained, which means we do not guarantee some free support. Consider reporting an [issue](#issues--features-request--proposal) and be patient. 

If you really like what we do or want to thank us for our quick work, feel free to [donate](https://www.paypal.me/BeAPI) as much as you want / can, even 1€ is a great gift for buying cofee :)

## License

BEA - PHP version is licensed under the [GPLv3 or later](LICENSE.md).

## Changelog ##

### 1.0.0
* 19 June 2018
* Initial