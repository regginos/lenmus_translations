lenmus_translations
===================

Translations of LenMus music training programme

Issues:
-------

Plural is not treated the usual way

Greek translation issues:
-------------------------

- When addressing the speach to the user the casual form should be used
  instead of the polite form.
  e.g. "You have the choice" 
  should be translated "Έχεις την επιλογή" 
  but not "Έχετε την επιλογή"
- The work "new" is used extensivly. We give preference to
  "νέο", "νέος", "νέα" over "καινούργιο", "καινούργιος", "καινούργια".
- "μείζωνα" or "μείζονα"?
- tuplet
- beam
- clef
- mode (λειτουργία ?)
- credits (συντελεστές ?)
- Licensed under
- Creative Commons Attribution/Share-Alike License;
- desktop (επιφάνεια γραφείου ?)
- Galician
- terminal/transient

Translation tips & tricks
-------------------------

Translate each .po file and provide a translation for each string using poEdit. If you are not sure with one or the other translation, mark it as fuzzy. You can enter a comment in poEdit to give some information about your thoughts to other translators. If you are not sure about the meaning of the original sentence post a message to the translators list and you will get more information.

To include a translation into the next LenMus release, at least the following files must be translated:

- lenmus_xx.po
- wxmidi_xx.po
- GeneralExercises_xx.po
- study-guide.htm

The first one (lenmus_xx.po) is the longest and the two last ones are very short. I recommend you not to start translating files:

- L1_MusicReading_xx.po
- L2_MusicReading_xx.po
- TheoryHarmony_xx.po

until the previous ones are ready.

File wxmidi_xx.po contains, mainly, the names of the 128 standard MIDI musical instruments. Probably you will be able to find somewhere, in Internet, this list in your language. This would save you some time in translation.

In strings to be translated you will find characters that have special meaning. Watch out for the following:

- In some strings you will find 'substitution marks' such as '%s', '%d' or '\n'. These represent places to include some data. They must be preserved in the translated string. Otherwise a compilation error will occur. As a special case, you will have to translate the following strings: 'c%d', 'd%d', 'e%d', ... 'a%d'. Please note that these strings represent the names of the notes followed by the substitution mark '%d'. So, for example, its translation in Spanish should be 'Do%d', 'Re%d', 'Mi%d', etc.
- Special characters such as quotes must be "escaped" (i.e. preceded with a backslash), if you want to use them as part of the text.
- The "&" character normally used to mark an "accelerator key", i.e. a letter which in combination with Ctrl (on PC keyboards) will execute the command; i.e. Ctrl + O for "Open file". You have to make sure that the same letter is not marked twice within one menu. The & can be placed before any letter, such us in 'Open s&pecial file'. In your translation, you should put the & before a suitable mnemonic letter for the menu function represented by the string, so that the chosen letter does not repeats in the same menu or submenu.
- Try to keep your translated string approximately the same size than the original. These is specially important in short strings used as labels for menus, buttons, etc. Otherwise, the translation might be too wide for the allocated space and the translated text will be cut off. If you find cases were the geometry of the offending buttons, menus, boxes, etc. is too short for the translation, please keep your translation and tell us by posting a message to the translators list, to create a new bug report.

For any problem you might have, please post a message to the translators list. Please, do not just leave the problem unmentioned. Thank you.


