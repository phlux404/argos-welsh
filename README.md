# argos-welsh

Welsh (Cymraeg) language packages for [Argos Translate](https://www.argosopentech.com/) / [LibreTranslate](https://libretranslate.com/).

## Packages

| Package | Direction | Size |
|---|---|---|
| `translate-en_cy-1_0.argosmodel` | English → Welsh | 78.9 MB |
| `translate-cy_en-1_0.argosmodel` | Welsh → English | 75.7 MB |

## Install

Once listed on the Argos package index:

```sh
argospm install translate-en_cy
argospm install translate-cy_en
```

Or install a package file directly:

```python
import argostranslate.package
argostranslate.package.install_from_path("translate-en_cy-1_0.argosmodel")
```

## Provenance

Converted from Helsinki-NLP's `opus-mt-en-cy` / `opus-mt-cy-en` models ([HuggingFace](https://huggingface.co/Helsinki-NLP)), released under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/). Packaged with the CTranslate2 / Locomotive pipeline and tested through argostranslate.

## Notes (v1.0)

- Full sentences translate cleanly in both directions.
- Very short fragments (a word or two, exclamations) can occasionally glitch — repeated or doubled words. That's small-model behavior, not a packaging bug.

A project by [phlux404](https://github.com/phlux404).
