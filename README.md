# Ansifin

This is a keyboard layout mainly aimed at people who are used to the [Finnish ISO layout](https://en.wikipedia.org/wiki/QWERTY#Finnish_multilingual) but want a layout that's better suited for software development and is more consistent between Windows and macOS on both common physical keyboard layouts, [ANSI and ISO](https://en.wikipedia.org/wiki/Keyboard_layout#/media/File:Physical_keyboard_layouts_comparison_ANSI_ISO_KS_ABNT_JIS.png).

<p align="center">(TODO: picture of the layout)</p>

The main features are:
* Access `[`, `]`, `{` and `}` from the same ergonomic spot as on the US and UK layouts.
* Access `<`, `>`, `/`, `|` and `\` consistently from the same keys no matter the OS or the physical layout you happen to be on.
* Access `ä`, `Ä`, `ö` and `Ö` from the same physical keys as the standard Finnish layout. `å`/`Å` is moved under Alt(Gr) because `[` and `{` are more important to most Finnish-speaking developers.
* Access the other characters the same way as on the standard Finnish layout on each OS.
* All the keys are in the same* places on both ANSI and ISO physical layouts.

If you don't care about the last point, you should also consider the [Finner](https://github.com/ruohola/finner) layout if that suits you better.

\*) Except **[**`* '`**]** because of, you know, geometry. The actual key still behaves the same.

## Installation

1. Download https://github.com/samulisuomi/ansifin/archive/master.zip
1. Unzip.
2. Install the layout for your OS:
   * macOS: Unzip `macOS\Finnish - US Influenced.bundle.zip` and then see e.g. [these instructions](https://weibeld.net/mac/custom-keyboard-layout.html) on how to install the `.keylayout` file found under `Contents/Resources`.
   * Windows: Run the installer from `Windows\finnishu\setup.exe`.
   * Linux: Sorry, no Linux version available as of now. :(

## Details

In many ways, the layout basically has the opposite philosophy compared to layouts like [Swerty](http://johanegustafsson.net/projects/swerty/) and [EurKEY](https://eurkey.steffen.bruentjen.eu/).

It's based on the standard Finnish keyboard layouts for Windows and macOS and does a few pragmatic changes to their four keys. These changes make room for the square and curly bracket characters to sit where they would sit on ANSI (on the **[**`å Å`**]** and **[**`¨ ^ ~`**]** buttons). Then the rest of the characters are shoved under shift and Alt(Gr) to keep them accessible. Finally, the positions of `<`, `>`, `/`, `|` and `\` are modified slightly to make them appear in the same place no matter what OS or the physical layout (ANSI or ISO) you are using.

Here's a list of the exact changes from the Finnish layout by each key. The standard PC naming is used but the Mac differences are highlighted on the individual character level:
- **[**`å Å`**]**:
  * normal press: `å` → `[`
  * shift + key: `Å` → `{`
  * Alt(Gr) + key: N/A → `å`
  * Alt(Gr) + shift + key: N/A → `Å`
- **[**`¨ ^ ~`**]**:
  * normal press: `¨` → `]`
  * shift + key: `^` → `}`
  * Alt(Gr) + key: `~` (not changed)
  * Alt(Gr) + shift + key: N/A → `^`
- **[**`§ ½`**]**:
  * normal press: `§` → `<`
  * shift + key: `½` (`°` on Macs) → `>`
  * Alt(Gr) + key: N/A → `§`
  * Alt(Gr) + shift + key: N/A → `½` (`°` on Macs)
- **[**`7 / {`**]**:
  * normal press: `7` (not changed)
  * shift + key: `/` (not changed)
  * Alt(Gr) + key: `{` (`todo` on Macs) → `|`
  * Alt(Gr) + shift + key: N/A (`todo` on Macs) → `\`

The layout files were created in [Ukelele](http://software.sil.org/ukelele/) and [Microsoft Keyboard Layout Creator](https://www.microsoft.com/en-us/download/details.aspx?id=22339).

## Dead keys

The characters with [dead key](https://en.wikipedia.org/wiki/Dead_key) behavior in the original Finnish layout behave the same way in this layout. For instance, hitting Alt(Gr) + **[**`¨ ^ ~`**]** doesn't print `~` before you also hit the space bar. However, both `]` and `}` (accessible via the same key) appear instantly (like on US ANSI).

A "no dead keys" variant may come in the future.

## Naming

The layout is still called `Finnish - US Influenced` in the downloadable layout files as I haven't had time to regenerate them with the new name. Sry.

## Limitations and caveats

* You completely lose access to `¨` compared to the original Finnish layouts (I'm sorrü).
* You will be able to enter some of the characters from multiple different keys (e.g. on Windows you can enter `\` both from the standard **[**`+`**]** key and from the new modified **[**`7`**]** key).
