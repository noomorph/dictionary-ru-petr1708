# dictionary-ru-petr1708

Russian (Petrine 1708 orthography) spelling dictionary.

## What is this?

This is a spelling dictionary of the Russian language in the Petrine 1708 orthography.
It is based on the [package](http://slavenica.com/za/?za=ru-petr1708-hunspell-3.1.tar.bz2) provided by [Slavenica](http://slavenica.com),
normalized and packaged so that it can be installed and used like other dictionaries.

## When should I use this?

You can use this package when integrating with tools that perform spell checking
(such as [`nodehun`][nodehun], [`nspell`][nspell]) or when making such tools.

## Install

In Node.js (version 14.14+, 16+ or 18+), install with [npm]:

```sh
npm install dictionary-ru-petr1708
```

## Use

```js
import dictionaryRuPetr1708 from 'dictionary-ru-petr1708'

dictionaryRuPetr1708(function (error, ru1708) {
  if (error) throw error
  console.log(ru1708)
  // To do: use `ru1708` somehow
})
```

Yields:

```js
{dic: <Buffer>, aff: <Buffer>}
```

Where `dic` and `aff` are [`Buffer`][buffer]s for `index.dic` and `index.aff`
respectively.

## Examples

See the [monorepo readme][dictionaries] for examples.

## Types

This package is typed with [TypeScript][].

## Contribute

Please [open an issue](https://github.com/noomorph/dictionary-ru-petr1708/issues/new) on GitHub.

## License

Dictionary and affix file: [MIT](https://github.com/noomorph/dictionary-ru-petr1708/blob/main/LICENSE).
Rest: [MIT][] © [Titus Wormer][home].

[hunspell]: https://hunspell.github.io

[nodehun]: https://github.com/nathanjsweet/nodehun

[nspell]: https://github.com/wooorm/nspell

[macos]: https://github.com/wooorm/dictionaries#example-use-with-macos

[npm]: https://docs.npmjs.com/cli/install

[dictionaries]: https://github.com/wooorm/dictionaries

[mit]: https://github.com/wooorm/dictionaries/blob/main/license

[buffer]: https://nodejs.org/api/buffer.html#buffer_buffer

[home]: https://wooorm.com

[typescript]: https://www.typescriptlang.org
