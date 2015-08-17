Character Limits and Typesetting Tests
-----------

Research on the typesetting and character limit issues found in the first English CBT for Tree of Savior. 

Includes screenshots.

For reference: According to [this,](https://en.wikipedia.org/wiki/Line_length) the **minimum comfortable reading width** for English text is a line width of **40 characters**, with an average of **~75 for books**, and **~100 for computer screens.**
The minimum of 40 characters is strict, as word wrap will begin to clash with the length of English words, creating a heavily jagged right margin.

### Summary

* All text appears to be left-aligned, non-justified.
* If word wrap is present, it is sometimes inconsistent with the boundary of the text box, creating cut-offs.
* Column width varies a lot, with about half dropping below 40 characters.
* Column height has different coding for different elements. Some are fixed; some are dynamic; some are dynamic, but requires line breaking with the {nl} tag.
* Some Unicode punctuation is supported, but this is actually dependent on the font file loaded.

* The game uses the font **Quattrocento Bold**. To check for available characters and to download a copy, go here: https://www.google.com/fonts/specimen/Quattrocento

### Specific Naming Limits

* **Items** — **20-35 characters.**
* **Skills** — **20-35 characters.**
* **Monsters** — **20-25 characters.**
* **Maps** — **4 words** if using a maximum of **10-12 characters per word.**

### Specific Images

* [Dialogue Boxes](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/dialogue.jpg) - **90 characters and 5 lines,** but oddly enough, there's a **hardcoded line break at 120.** Very long lines will automatically continue into a new box. After comparing it to an older screenshot from imc taken before the CBT, it looks like the font size has been raised.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/dialogue.jpg" height="192" >
<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/dialogue-imc-pre_cbt1.jpg" height="96" >

* [Unicode, Alphabet and Appearance](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/unicode%20test.jpg) - A pangram is a phrase that uses the language's entire alphabet. All the basics for English and German are in here, as well as basic Unicode punctuation. I used {nl}'s, and you can see that there is actually a sixth line, that cuts off after one character. The character is repeated in the next window. Almost all Unicode failed, but this is usually caused by the font file that's loaded. The full character limits can be checked at https://www.google.com/fonts/specimen/Quattrocento

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/unicode%20test.jpg" height="192" >

* [Unicode and Alphabet (Short)](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/unicode%20test%20-short.jpg) - The two failed characters in the second line are the reverse quotes, and I don't think anyone really uses those. Also, I have included a three-period-character ellipsis in the first line, while the second line has the Unicode ellipsis. You people debate far too much about them.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/unicode%20test%20-short.jpg" height="128" >

* [Character Creation](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/char%20creation.jpg) - **60 characters, 7 lines.** Class summaries at the moment are only 2-3 lines, creating a lot of whitespace.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/char%20creation.jpg" height="192" >

* [Floating NPC Names](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/dialogue%20pick.jpg) - **45 characters, with lines added with {nl}.** However, extra lines are currently left-aligned, and manual indenting is required to center the text.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/dialogue%20pick.jpg" height="128" >

* [Dialog Prompts (seen above)](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/dialogue%20pick.jpg) - **~60 characters, one line.** Many, many lines are actually Player lines, which means quotation marks need to be added.

* [Help Bubbles](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/help%20bubble.jpg) - **30 characters, 2 lines.** When the text was reloaded, it jumped upward on the screen for some reason.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/help%20bubble.jpg" height="128" >

* [Help Screen](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/help.jpg) - **50 characters, with dynamic height.** The top blurb above the scroll has a fixed limit of 4 lines. The text on the list disappears when the .tsv files are reloaded.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/help.jpg" height="192" >

* [Loading Screens](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/loading.jpg) - **dynamic width and height.** However, the text is left-aligned and had a centrally aligned box.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/loading.jpg" height="192" >

* [Item Descriptions](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/item%20desc%20popup.jpg) - **45 characters and dynamic height**, with good word wrap. 

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/item%20desc%20popup.jpg" height="192" >

* [Skill Descriptions](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/skill%20desc%20popup.jpg) - **35 characters** for the upper part, **30 characters** for the lower part. Overall, the margins are extremely large and could use a new layout.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/skill%20desc%20popup.jpg" height="192" >

* [Quest Info](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/quest.jpg) - **45 characters, with dynamic height.** Word wrap is still cutting some long words off.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/quest.jpg" height="192" >

* [Quest Info Hint](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/quest%20hint.jpg) - **40 characters with dynamic height,** and the Quest Name at **38 characters.** Word wrap margin appears to actually be oversized to 45, even though the box has a size of 40, creating cutoff.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/quest%20hint.jpg" height="192" >

* [Quest Clear](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/quest%20clear.jpg) - **45 characters** like the other quest stuff.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/quest%20clear.jpg" height="192" >

* [Tooltips](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/tooltip%20with%201%20nl.jpg) - **infinite width, and no word wrap.** One {nl} tag was used. Also, it looks like tooltips are being abused throughout the game, with many 6-7 line tooltips.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/tooltip%20with%201%20nl.jpg" height="96" >

* [Hotbar](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/hotbar.jpg) - **4 characters.** It's usually not a surprise to get text overrun here. The shift key has a custom shortening, but Numpad does not.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/hotbar.jpg" height="128" >

* [Book View](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/book%20view.jpg) - **35 characters, one page ~512 characters.** The font size is too large. There is also an unknown additional hardcoded break at 425 characters, and hardcoded breaks continue across many pages. Also, many books only have 1 sentence per pages, leading to a lot of empty space.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/book%20view.jpg" height="256" >

* [Item Pop-Ups](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/item%20get.jpg) - **~20 characters.**

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/item%20get.jpg" height="192" >

* [Monster Names](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/monstername.jpg) - **~20-26 characters**

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/monstername.jpg" height="96" >

* [World Map Titles](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/world-map-titles.jpg) - **approx. 1 long word per line, 5 lines.** Since the Level Requirement is also on the title, this means map names should never exceed three or four words, of reasonable length.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/world-map-titles.jpg" height="128" >

* [World Map Pop-Ups](https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/map-popup.jpg) - Didn't check for strict limits, but there are **problems with overlap and cutoff,** due to the layout and name length, depending on the map.

<img src="https://raw.githubusercontent.com/ensata/TreeOfSavior-en-research/master/interface%20research/map-popup.jpg" height="192" >