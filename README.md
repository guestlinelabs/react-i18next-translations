# Translation Hover Extension for React i18next

## Overview

This extension provides hover information for translations in your VS Code project.
It recognizes translation keys while using i18next for react and displays their corresponding translations as a hover message.

## Features

- Hover over a translation key in your code to see its translation in english.
- Automatically finds the nearest translation file based on your project structure.
- Supports:
  - `t("fileName:translationKey")`
  - `t("fileName:translationKey.nestedTranslationKey")`
  - `t("translationKey")` - while using `const { t } = useTranslation("fileName")`
  - `i18nKey="fileName:translationKey"`

## Usage

1. Provide correct paths to your translations folders related to root of your react project.
2. Provide correct settings in `settings.json` e.g.:
   `{"reacti18nextTranslationOnHover.defaultLocale": "en-GB",
"reacti18nextTranslationOnHover.translationFolderPaths": ["translations", "public/translations"]}`
   By default locale is set to be `en-GB` and folders to be `["translations",
"public/translations",
"public/locales"]`
3. Hover over a translation key to see its translation.
