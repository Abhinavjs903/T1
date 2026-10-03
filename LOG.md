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

## CC-03 — "The menu is wider than my phone"

**Reproduced:** Entered the mobile (320px) and moved to the tabs which were not completely visible

**Cause:**The width of the cards were set to max content and getting into extended horizontal side

**Fix:** fixed the width and cross checked the width % of others

**Checked:** Checked after updating the code, the cards were correctly visible

**Time:** about 30 mins in identifying code and rule in the style.css


## CC-04 — "The buttons don't work on my tablet"

**Reproduced:** Entered the tablet width range (761–900px) where the Add to Cart and star buttons were not working, while they worked on other screen sizes.

**Cause:** An invisible layer created by the tablet-specific CSS was covering the buttons and blocking the click events.

**Fix:** Added pointer-events: none to the invisible layer so that it does not block clicks on the buttons.

**Checked:** Checked the buttons again after updating the CSS. Add to Cart and star buttons were working correctly on the tablet dimensions.

**Time:** about 45 mins in identifying the tablet-specific CSS block and invisible layer in the style.css

## CC-05 — "The category bar scrolls away on my phone"

**Reproduced:** Shifted into the phone dimensions and found that cat-tabs and filters were going up with the scroll

**Cause:** the postition of filters file was set to relative and it depended and not fixed so it moved up with the scroll

**Fix:** Adjusted the positioning and fixed it on the page then also managed further elements around it which was going hidden and provided a padding to it too

**Checked:** Veridied cat- tabs and filters is moving constantly with screen and lined up with the top

**Time:** 20 mins finding the bug and adjusting the proper elements


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
