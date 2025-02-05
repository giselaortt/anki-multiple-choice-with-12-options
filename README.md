<!-- omit in toc -->
# anki-mc

# Credits:
original work from: https://github.com/zjosua/anki-mc

# anki multiple choice with 12 options

This is my version of zjosua work.
Thiss add on allows for multiple choice on anki, but only 5 options. For some german declinations I needed up to 8 diferent options in order to contain every declination. So I changed the original code and increased the possibility to 12 options (a bit extra just in case).

I also changed the colors to less bright ones for personal preference.
=======
- [Screenshots](#screenshots)
- [Compatibility](#compatibility)
- [Usage](#usage)
  - [Creating / Editing](#creating--editing)
  - [Reviewing](#reviewing)
  - [Addon Config](#addon-config)
  - [Known Issues](#known-issues)
- [License and Credits](#license-and-credits)

## Screenshots

|                  Single Choice                  |                   Multiple Choice                   |              Kprim              |
| :---------------------------------------------: | :-------------------------------------------------: | :-----------------------------: |
| ![Single Choice](screenshots/single_choice.png) | ![Multiple Choice](screenshots/multiple_choice.png) | ![Kprim](screenshots/kprim.png) |

## Compatibility

Anki 2.1.55 or higher is required for the most recent version of this add-on to work.
For Anki 2.1.44 to 2.1.54, you can use v2.8.0 (or lower) of the add-on.
>>>>>>> 5ce2159cf50744618e1ba39003ef7af32c45ac79

License kept from original work.

### How to use ?


the only folder that actually matters is the "multiple-choice" folder inside "src". You just need to add this one to your add-on folder.

alternativelly you can add it trhought the anki add-ons tool, using the code 1573325751. my add-on link is this: https://ankiweb.net/shared/info/1573325751

<<<<<<< HEAD
=======
## Usage
>>>>>>> 5ce2159cf50744618e1ba39003ef7af32c45ac79

### Creating / Editing

The note type is automatically added the first time you start Anki after installing the add-on.

When creating cards, write a "1" for correct choices or a "0" for incorrect choices in the "Answers" field.
The question type can be selected with the field "QType".
It can be either 0 (Kprim), 1 (Multiple Choice) or 2 (Single Choice).
The [Screenshots](#screenshots) section shows how the question types look.
These values in the "Answer" field must be separated by a single space.
The order and number of values in the "Answer" field must correspond with the choices "Q_1" to "Q_5".
If you don't need all the choices, just leave the remaining "Q_" fields blank and only enter as many values as you need in the "Answers" field.


<<<<<<< HEAD
### License and Credits -> original text from zjosua
=======
### Reviewing

Select the correct and incorrect choices accordingly and click "Show Answer".
The add-on will automatically style your choices based on whether you answered correctly or not.

### Addon Config
>>>>>>> 5ce2159cf50744618e1ba39003ef7af32c45ac79

If you want to change the way your answers are styled (e.g. color green what you should have chosen instead of what you have chosen correctly) you can use the addon's config to switch between different styles:
![Addon Config Window](screenshots/addon_config.png)
(Tools -> Addons -> "Select the multiple choice addon" -> Config)


### Known Issues
- [I don't understand the colors](https://github.com/zjosua/anki-mc/pull/90)
  - Use the [addon's config](#addon-config) with `ALTERNATE_COLORING`
- [Turn off shuffling/randomization of answers](https://github.com/zjosua/anki-mc/issues/87#issuecomment-1259818989)
  - Possible by duplicating the note type `AllInOne (kprim, mc, sc)` and replacing `qanda = shuffle(qanda);` with `// qanda = shuffle(qanda);`.
- [More than 5 answer options](https://github.com/zjosua/anki-mc/issues/81)
  - Possible with slight modification of the note type (fields) and tempalte HTML

## License and Credits

*Multiple Choice for Anki* is *Copyright © 2023 [3ter](https://github.com/3ter) and [zjosua](https://github.com/zjosua)*

It is licensed under the AGPLv3.
For more information refer to the [LICENSE](https://github.com/zjosua/anki-mc/blob/master/LICENSE) file.

A bunch of code in this add-on is based on the Anki add-ons [Image Occlusion Enhanced](https://github.com/glutanimate/image-occlusion-enhanced) and [Cloze Overlapper](https://github.com/glutanimate/cloze-overlapper) by Glutanimate.
[Click here to support Glutanimate's work](https://glutanimate.com/support-my-work/).

Persistence is achieved using the code from [Simon Lammer's anki-persistence](https://github.com/SimonLammer/anki-persistence).
Great work Simon!

[Hax](https://github.com/Schlauer-Hax) merged my Multiple Choice card template with Simon Lammer's persistence code.
He also reworked my card templates into one single all-in-one template.
Thanks a lot!

Simon's and Hax's work made the multiple choice cards compatible with all platforms.

Volker Umpfenbach contributed a change that allows to customize how the questions and answers are colorized.
He also provided the code to calculate and display the percentage of correctly answered items per question.

This add-on uses the [packaging](https://packaging.pypa.io/en/latest/) library.
