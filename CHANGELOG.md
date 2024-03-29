# Changelog

## 0.3.4

- Fixed dependencies listed in package.json. See
  https://github.com/j0lv3r4/mdx-prism/issues/8

## 0.3.1+fork.0.1.0

- Fork from @mapbox/rehype-prism
- Add markers following react-refractor example
- Add highlight line support following gatsby-remark-prismjs example

## 0.3.1

- Allow uppercase language names in the `language-*` class (e.g. `language-CSS`).

## 0.3.0

- Add `language-*` class to the `<pre>` tag of the output, because many Prism themes rely on this undocumented pattern.

## 0.2.0

- **Breaking:** Add `options.ignoreMissing` which defaults to `false`.
  If you are relying on *silent* failures to highlight when the language is not defined, you'll need to use this option.
- **Breaking:** Remove support for `nohighlight` and `no-highlight` classes.
  You can skip highlighting for any given `<code>` by *not* putting a `language-*` class on it.
- Under the hood, use [refractor](https://github.com/wooorm/refractor) instead of Parse5 and PrismJS directly.

## 0.1.0

- Initial release.
