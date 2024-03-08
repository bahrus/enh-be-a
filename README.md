# enh-be-a [TODO]

*enh-b-a* allows us to subclass an existing custom element, unchanged, and just give it a more meaningful name, depending on the context.  This allows us to make our HTML markup more semantic.

For example, suppose we hav a generically named web component, like ["time-ticker"](https://github.com/bahrus/time-ticker).

We wish to use that web component, but give it a more meaningful name.  We can do that thusly:

```html
<message-rotator enh-be-a=time-ticker></message-rotator>
```

Only one such instance need to be adorned, and it subsequent instances will work throughout the (scoped) application without the registering hint.