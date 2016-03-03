The Quick Tabs Field Collection module provides a field formatter for rendering [field collections][1] as [Quick Tabs][2].

## Requirements

* [Field Collection][1]
* [QuickTabs][2]

## Related

[Field Collection Tabs][3] is a module with similar functionality. It renders a field collection as tabs, whereas this module uses Quick Tabs to render a field collection.

## Usage

1. Go to the Manage Display page for any Entity that contains a field-collection field.
2. Change the formatter to QuickTabs
3. Click the gear icon on the right to access the formatter settings.
  * (REQUIRED) Enter the machine-name of the field to use for the tab values.
  * (REQUIRED) Enter the machine-name of the field to use for the tab contents.
  * Optionally tick the box to strip all HTML tags from the tab content.
  * Optionally add custom classes that will output in the field-collection wrapper div.
  * Optionally configure the available QuickTabs options.
4. Adjust formatter settings for each of the fields in the field-collection.

  The field used to output the value of the tab label and tab contents respects the formatter settings applied to those fields. However any HTML that is output get in the tab label is run through `check_plain()` by the QuickTabs module so it is recommended to choose Plain Text as the formatter for the tab value.

[This issue][4] contains screenshots that may better illustrate the above.

[1]: http://drupal.org/project/field_collection
[2]: http://drupal.org/project/quicktabs
[3]: http://drupal.org/project/field_collection_tabs
[4]: http://drupal.org/node/1902254#comment-7000450
