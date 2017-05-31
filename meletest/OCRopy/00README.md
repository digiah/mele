#OCRopus

## method
Initial simulations used all but last three lines of the first page for training and applied the resulting model to those last three lines.
The trainings were run on each of the three suffix sets below.
The training set is insufficient here, but should be sufficient for illustration purposes.

## file name key for input files

* no suffix: Umesh's original transcriptions
* suffix "-1.txt" = no unicode except okina, transcriptions corrected
* suffix "-2.txt" = unicode font substitutions for diacritic marks, transcriptions corrected. For unicode characters in use, see [00-UnicodeUsed.txt](00-UnicodeUsed.txt) in this folder.
* suffix "-3.txt" = no unicode font substitutions at all, typewriter only, transcriptions corrected

## results

* The recognition of the unicode characters (suffix 2) was not successful with the limited training set. A larger training set might resolve this.  
* For text that does not utilize unicode characters except for okina (suffix 1), recognition is better but okina is swapped for tilde.  A larger training set might resolve this.
* For typewriter characters only, no unicode (suffix 3), including using apostophe (') rather than okina (ʻ), the recognition was excellent even with the small training set.  Only one uppercase K mistranslated.  A larger training set would definitely correct this.
