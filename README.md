# Waiting for Godot Processed Text
Waiting for Godot by Samuel Beckett

Content retrived from Samuel Beckett's website.

There are total of 2 acts and therefore 2 pages.
http://www.samuel-beckett.net/Waiting_for_Godot_Part1.html
http://www.samuel-beckett.net/Waiting_for_Godot_Part2.html

The original HTML has some missing tags and wrong encoding.
Chrome seem to fix it when parsing it and I save the version fixed by Chrome, and change the encoding to UTF-8.
They are saved as wfg1.html and wfg2.html

The two saved HTML pages then parsed with BeautifulSoup. And I wrote some code to eliminate the non-dialog parts. Luckily they are either italic or encapsualted in a blockquote tag.

The detailed Process can be found inside the two notebooks.

## Preview
```
ESTRAGON: Nothing to be done.
VLADIMIR: I'm beginning to come round to that opinion. All my life I've tried to put it from me, saying Vladimir, be reasonable, you haven't yet tried everything. And I resumed the struggle. So there you are again.
ESTRAGON: Am I?
VLADIMIR: I'm glad to see you back. I thought you were gone forever.
ESTRAGON: Me too.
VLADIMIR: Together again at last! We'll have to celebrate this. But how? Get up till I embrace you.
ESTRAGON: Not now, not now.
VLADIMIR: May one inquire where His Highness spent the night?
ESTRAGON: In a ditch.
VLADIMIR: A ditch! Where?
ESTRAGON: Over there.
```

## Use
The two html pages has two output wfg1.txt and wfg2.txt respectively.

I have also extract a scene of the text according to scenes divided from this pdf
http://www.itisrighi.fg.it/public/26/home/503_waitingforgodot.pdf

Hence, both wfg1 and wfg2 has a train and test version as well. It was intended to be fine-tuned with GPT-2.

Finally, a combined version is created:

wfg1 + wfg2 -> wfg

wfg1train + wfg2train -> wfgtrain

wfg1test + wfg2test -> wfgtest