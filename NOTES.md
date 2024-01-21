# Notes

JGhali in the bug tracker: You have to download the required hyphenation and spelling dictionaries. You can do so from Windows > Resources menu. Hyphenation and spelling dictionaries for German (Austria) are not provided by default. 

[Uflanusi wrote](https://forums.scribus.net/index.php?msg=22467):

```
I recently had the same problem and found the following solution on my Linux Fedora System:
Like the others, I also did not have a dict file in /usr/share/scribus, and could not use hyphenation in scribus with my selected language (german)
but as hyphenation did work with english words although there is no dictionary file, i assumed Scribus shares the language-hyphenation-files with other programs.


I installed the following package via my package-manager: hyphen-de.
(before that, I also installed hunspell-de,  but I think this was not necessary).
And now it works!

To check whether your language-hyphenation-rule is missing on linux-fedora use the following command:

dnf list installed | grep 'hyphen'

output:
hyphen-de
hyphen-en
etc.

Also check the following in scribus:

- Is hyphenation activated for the project/file? (  "File > Document Setup > Hyphenator > checkboxes")

- Did you assign the right language ( hyphenation rules) to the selected textframe (in "edit > styles > paragraph styles > character style tab" , or directly for the selected textframe in the text properties)?

- Select the textframe and navigate to "Extras > Hyphenate Text"



links:
https://wiki.scribus.net/canvas/Help:Manual_HyphenatioN (some points outdated)
```
