# enh-be-a [TODO]

*enh-b-a* allows us to subclass an existing custom element, unchanged, and just give it a more meaningful name, based on the context in which it is used.  This allows us to make our HTML markup more semantic.

For example, suppose we have a generically named web component, like ["time-ticker"](https://github.com/bahrus/time-ticker).

We wish to use that web component, but give it a more meaningful name.  We can do that thusly:

```html
<message-rotator enh-be-a=time-ticker></message-rotator>
```

Only one such instance needs to be so adorned with the attribute -- subsequent instances will work throughout the (scoped) document without needing to add the registering hint.  But no harm done if it is added anyway.