# New installation


## Standardintegration

Dieses Modul ist ab der Shopversion 1.2.0 im Standard integriert und muss nur im Adminbereich oder der Kommandozeile [aktiviert](#Aktivierung) werden.

## Systemanforderungen

- O3-Shop ab Version 1.2.0
- Composer
- PHP 7.4 oder höher

## Installation

Wenn das Modul nicht installiert ist, können Sie dies nachholen.

For a new installation of the editor plugin you need Composer. See under [Server and System Requirements](#SystemRequirements) section [Composer](SystemRequirements.md#composer).

For installation instructions, see the Getting Started section of the Composer pages at [https://getcomposer.org](https://getcomposer.org).

Führe den folgenden Befehl auf der Kommandozeile aus: 

```
composer require o3-shop/tinymce-editor
```

## Aktivierung

Aktivieren Sie das Modul im Adminbereich unter "Erweiterungen -> Module -> TinyMCE Editor".
Leeren Sie anschließend den TMP Ordner.