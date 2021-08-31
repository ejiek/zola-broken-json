# Zola json field access bug MVP repository

Sole purpose of this repository is to be a demo for [zola/#1605 issue](https://github.com/getzola/zola/issues/1605).

In a current state it's not building because zola can't access a field that doesn't exist (due to a bug).
Changing variable access to the context output in `templates/shortcodes/broken.html` shows that a json file is parsed correctly.

```
{{ broken_json.bro-ken }}
```

to

```
{{ __tera_context }}
```
