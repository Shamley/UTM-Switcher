### UTM Switcher

The UTM Switcher is a powerful tool to help you track _where_ your site visitors are coming from and modify page elements based upon a utm_source GET variable in a url. It notes where a site visitor first lands, and then proactively changes targeted elements across your entire website to match that source.

### Keep track of your leads

In digital marketing, it can be difficult to figure out which of your channels is getting the best results: whether it’s Adwords, facebook paid advertising, blogging, or something else. For this reason, some companies use landing pages with different phone numbers to track the source of a lead. However, typical customers have multiple interactions with a site before following any call to action. They may click through several pages before making a decision. That’s where UTM Switcher comes in.

### How it works

UTM Switchers uses cookies to keep your lead-specific content consistent across all pages. The cookies are only destroyed once the website is closed. It works with all Wordpress sites and features integrations with Contact Form 7 and Contact Form DB. The information stored is taken from the URL's GET variables utm_source, utm_medium, and utm_campaign

When a UTM Switcher finds a matching DOM element using jQuery, it replaces the content of that element with the value supplied in the switch. Each Switcher can be set to match a specific utm_source in the URL or stored as a cookie value to the specific DOM element. An example of this is if the utm_source value is Facebook change the value to 1234 and if the utm_source value is Twitter change the targeted element to 4321. Each Switcher can also be set to replace the value with a tel: anchor tag for use with a call tracking plugin.

You can read more about the [call tracking plugin here](https://www.betoplocal.com/call-tracking-plugin/).

### Required PHP version
PHP 5.4 or greater

### Required plugins

None

### Recommended plugins

Contact Form 7 - If you choose, the UTM information can be sent in your form email. This information will include the information gathered from the initial URL GET variables utm_source, utm_medium, and utm_campaign. These values are then passed along to the email via a shortcode, e.g. [utm-100] 

Contact Form DB - This extension is not required, but we do recommend it.

### Usage

To use a UTM Switch:

1. Under UTM Switchers, click Add New
1. Enter an Identifier -- this is for internal use only. You could use it to keep track of what the switch does.
1. Enter an selector (an #ID or .classname or other selector) to target. This field uses [jQuery syntax](http://api.jquery.com/category/selectors/).
1. Choose the Type. Phone Number Element will replace the whole element with an anchor link with a tel: attribute. Text replacement replaces all text in the above element.
1. Click "Add Switcher" under UTM Source Switchers. A matching value in the Campaign Source field to the utm_source GET variable will replace the above selector's content with the value in the Replacement Value field. HTML can be used. You may add multple switches for different UTM Sources.
1. Click Publish.