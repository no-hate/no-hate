# NoHate

> The goal for NoHate is to reduce the number of mean comments
> for bloggers and news outlets

### Basic installation instructions

1. Find the id / selector of your comment field.
   1. Open up your site and navigate to a page with comments.
   2. Right click on the comment field and click 'Inspect'.
   3. Right click the element in the inspector window, and click Copy > Copy selector.
2. Copy the code below, and modify the settings to fit your needs.
3. Paste the code right before the bottom of the &lt;body&gt; tag on the template page(s) that has comments.

### Plugin options

All settings are optional - default are specified below.

- `field`
  selector for the textfield you want to target

  > default: '#comment'

- `language`
  the language file to use

  > default: 'no' // Norwegian

- `custom`
  custom words

  > example: ["giraffe", "cantaloupe"]
  > default: N/A

- `verbose`
  enable verbose logging

  > default: false

### Typical plugin configuration

```html
<!-- NoHate Plugin -->
<script src="https://cdn.jsdelivr.net/gh/no-hate/no-hate/nohate.min.js"></script>
<script>
  NoHate.init({
    field: "#comment"
  });
</script>
```

### Including the plugin on your site

Paste the code right before the bottom of the &lt;body&gt; tag on the template page(s) that has comments.

### Verify that the plugin is working

To verify that the plugin is working, visit your website and enter `NoHateVerify` into the targeted textarea and click submit.

### Anonymized analytics events tracked by the plugin

- `Initializing`
  when the plugin is initializing

  > value: true

- `Initialized`
  when the plugin is connected to an inputfield / textarea

  > value: true / false

- `Load`
  when the language file starts loading

  > value: language

- `Valid`
  when the plugin is validating a comment

  > value: true / false

- `Cancel`
  when the user clicks go back / outside popup

  > value: true

- `Submit`
  when the user clicks "post comment"

  > value: true

- `Report`
  when the user clicks "report error"

  > value: true
