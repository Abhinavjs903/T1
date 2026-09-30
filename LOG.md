# Debug log

Your notes. One entry per bug you fixed, using the template below.

This file is read as carefully as your code. A correct fix you cannot
explain counts for little; a bug you could not fix but investigated
honestly still counts for something.

Delete the example before you submit.



## CC-01 — "The search suggestions are behind everything"

**Reproduced:** Tried searching for several food itams but the suggestion list was behind the cat tabs

**Cause:**The stacking value for all the tabs , (cat-tabs) ,.search-wrap are mismatched

**Fix:** Checked and experimented the values in the website and updated the new stacking rule

**Checked:**Updated working and the suggestion box and search wraps

**Time:** about 15 mins in identifying code and rule in the style.css

## CC-02 — "Can't read anything in dark mode"

**Reproduced:**Swtched to Dark Mode and checked the food tables of all and can't read the text there.

**Cause:**The dish tabs' colour was fixed to dark only while it was supposed to be fixed only on the theme on the ink

**Fix:** Changed the ink colour to be theme dependent [var(--ink)]

**Checked:** hard refreshed and verified the dish tabs' colours

**Time:** about 15 mintues figuring out the bus , and checked it's function



## Could not fix

For anything you investigated but did not solve. Say what you tried and
where you got to. This is worth marks — leaving it blank when you got
stuck is not.

### CC-0X — "<the complaint>"

**What I tried:**

**Where I got to:**

**What I would try next:**



## Extra credit

Anything not on the bug log: a problem you found yourself, a test you
wrote, or a fix you are unsure about. Same format, plus one line on how
you noticed it.
