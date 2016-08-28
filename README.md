## Inspiration
After learning about how Markov Chains can be used to simulate language, I became fascinated with the idea of "seeding" Markov Chains with interesting corpuses for entertainment purposes.

## How to Use TextToMarkov
Examples of how each of the functions in textToMarkov.py should be used are in the main function of textToMarkov.py.  In Summary:
- 1) Run setup() to create "corpuses" and "pickles" folder.
- 2) Run loadData('corpuses.txt', True) to load data from corpuses.txt and save generated data structures for future use.  After this, you can run loadData('corpuses.txt') or loadData('corpuses.txt', False) to read in data structures that have been generated previously.  This saves time as the entire .txt file doesn't need to be read in and reprocessed over and over again.
- 3) Run createSentence() to generate a sentence based on the Markov model.

## Other
- 1) textToMarkov.py can only read in .txt files
- 2) textToMarkov.py will generate as much of a complete sentence as possible using a 2-gram Markov Chain.  If the script gets "stuck", it will revert to a 1-gram Markov Chain to generate the next word in the sentence, and then will continue using the 2-gram Markov Chain model.

## Sentence Examples
Some fun sentence examples are as follows.  The corpus used is listed after each:
- 1) "7:28 and their word will eat as doth a fool than of the oppressor?" (kingJamesBible.txt)
- 2) "With grief, yea, my heart was darkened." (kingJamesBible.txt)
- 3) "To milan let me kiss my hand, make signal of my womb, my womb, my womb, my womb undoes me." (shakespeare.txt)
- 4) "I wooed for the ma glorify the banks that bound them and my soul to that name the mothers still their babes." (shakespeare.txt)
- 5) "I challenge anyone to explain the strategic foreign policy disaster after another." (trumpSpeeches.txt)
- 6) "Brady loves me and he loves you." (trumpSpeeches.txt)

## Sources
I downloaded the corpuses from the following sites:
- 1) trumpSpeeches.txt from https://github.com/ryanmcdermott/trump-speeches/blob/master/speeches.txt
- 2) shakespeare.txt from http://ocw.mit.edu/ans7870/6/6.006/s08/lecturenotes/files/t8.shakespeare.txt
- 3) kingJamesBible.txt from http://www.gutenberg.org/cache/epub/10/pg10.txt
