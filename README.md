# Vocabulary: Learn and Test

**Five expert English words a day.**
Developed by **Dr. V C Srivastava**.

Vocabulary: Learn and Test is a small web app that you can install on a phone. It runs on GitHub Pages at
https://vcsrivas.github.io/wordtrio/

## Disclaimer

This app has been made using an AI platform. Although much care has been taken for its correctness, it may still contain errors, so please use it with caution and check important words in a standard dictionary.

## What it does

- Shows **five words a day**, picked at random from the 4,397 words in `words.xlsx`, including words taught in *Word Power Made Easy* by Norman Lewis and words listed in *Roget's Thesaurus of Words for Writers* and *The Oxford Thesaurus*. Every word is of the level tested in competitive examinations such as IPMAT, CAT, GRE and SAT; technical, archaic, dialect and informal words have been left out.
- No word is repeated until every word in the list has been shown.
- Each word shows its part of speech, meaning and a usage example, and, where available, other meanings and synonyms. Tapping a synonym lets you look it up in Oxford or Cambridge.
- Every word has **Oxford** and **Cambridge** buttons that open its entry on those dictionaries' websites.
- **History** lists the words shown on the phone each day. Tap any word to see its full card, with the dictionary buttons. Words answered wrongly in tests are listed at the top under *Words to revise*.
- The sections **Today**, **History**, **Practice Test**, **Quiz** and **Search** are in a strip on the left of the screen, with the names written upwards (first letter at the bottom) and the icon at the start of each name. **About** opens from the ℹ️ button at the top right.
- **Search** works both ways: type a word to find its card, or type a word from a meaning (such as *angry* or *praise*) to find the words with that meaning or synonym. Suggestions appear as you type.
- **Practice** gives a test of 10, 20, 30 or 50 questions from the whole list, each with four options. There are three kinds of question: word → meaning, meaning → word, and fill in the blank (using the word's usage sentence). There is also a *Practise my mistakes* test.
- **Quiz** gives the same kinds of test, but only on the words already shown in the daily cards.
- Scores of every practice test and quiz are saved on the phone, with the number of tests, the average, the best score and the last ten results.
- **Control panel:** add `#control-panel` to the end of the app's address to open it. It shows every screen. Tap any part of a screen (a tab, the left strip, a heading, a button, any text) to change just that part: its background, text colour, border, font, text size, thickness, slant and corner roundness. You can also choose a ready-made theme and change any colour (also for dark mode), the fonts, text size, word size, corner roundness and the left-strip width. Press **Copy theme.css** and paste the text into `theme.css` in this repository to change the look for everyone.
- A day streak counts how many days in a row the words have been opened.
- It can be installed to the home screen and opens like an app. The tabs, colours and fonts follow the Hindi-English dictionary app (navy theme, Mukta font), with a dark mode.

## Files

| File | Purpose |
|---|---|
| `index.html` | The app |
| `theme.css` | The app's colours, fonts and sizes (made with the control panel) |
| `control-snaps.json` | Sample screens shown in the control panel |
| `words.xlsx` | The word list |
| `manifest.webmanifest`, `sw.js`, `icons/` | Make the app installable and let it open offline |

## Updating the word list

Replace `words.xlsx` in this repository with a new file of the same name. The app reads the tab whose header row has **Word** and **Meaning** columns. Recognised columns are:

Word, Part of Speech, Meaning, Usage (example), Other Meanings, Synonyms.

Other Meanings are separated by ` | `, and each can start with a part of speech such as `(nou.)`, `(adj.)`, `(ver.)` or `(adv.)`. Synonyms are separated by commas.

## Acknowledgements

Most meanings, synonyms and other meanings in `words.xlsx` (1,662 words) come from **Princeton WordNet**, the lexical database of English created at Princeton University. Usage examples come from WordNet where it has one (594 words); the other examples were written for this app with the help of AI.

The list also includes words taught in *Word Power Made Easy* by Norman Lewis and words listed in *Roget's Thesaurus of Words for Writers* by David Olsen, Michelle Bevilacqua, Justin Cord Hayes and Robert Bly, and headwords from *The Oxford Thesaurus: An A–Z Dictionary of Synonyms* by Laurence Urdang, as well as the words in Dr. V C Srivastava's own Word Power list. Only the words are taken from these books; none of their definitions, synonym lists or example sentences are used. For 2,735 of these words that are not in the WordNet file, the meaning, synonyms and example were written for this app with the help of AI. The **Meaning Source** and **Example Source** columns in `words.xlsx` show which is which.

> WordNet 3.0 Copyright 2006 by Princeton University. All rights reserved.
> Used under the WordNet 3.0 licence (https://wordnet.princeton.edu/license-and-commercial-use).

The WordNet data was taken from **Open English WordNet** (https://github.com/globalwordnet/english-wordnet), the open-source edition of Princeton WordNet, released under the Creative Commons Attribution 4.0 International licence (CC BY 4.0).

Word frequency scores, used only to choose expert-level words, come from the OpenSubtitles 2018 frequency list (https://github.com/hermitdave/FrequencyWords, CC BY-SA 4.0).

### References

- Lewis, Norman. *Word Power Made Easy*. (Source of some of the words in the list; no text from the book is used.)
- Urdang, Laurence. *The Oxford Thesaurus: An A–Z Dictionary of Synonyms*. Oxford University Press. (Source of some of the words in the list; no text from the book is used.)
- Olsen, David, et al. *Roget's Thesaurus of Words for Writers*. Adams Media. (Source of some of the words in the list; no text from the book is used.)
- Princeton University. "About WordNet." *WordNet*. Princeton University, 2010. https://wordnet.princeton.edu/
- Miller, George A. (1995). "WordNet: A Lexical Database for English." *Communications of the ACM*, 38(11), 39–41.
- Fellbaum, Christiane (ed.) (1998). *WordNet: An Electronic Lexical Database*. Cambridge, MA: MIT Press.

Cambridge Dictionary and the Oxford Learner's Dictionaries are only linked to. None of their content is copied into this app.
