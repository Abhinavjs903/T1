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

## CC-06 — "I ordered more than they had"

**Reproduced:** Tried to place an order with a quantity greater than the available stock. The order was successfully placed.

**Cause:** The condition was not checking whether the requested quantity was greater than the available stock.

**Fix:** Added a stock quantity validation so the order is rejected when the requested quantity is greater than the available stock.

**Checked:** Tested with a quantity greater than the available stock and the order was rejected with an invalid order message. Also tested with a valid quantity and the order was placed successfully.

**Time:** about 20 mins in identifying the validation logic and testing the fix

## CC-07 — "Cancelling makes stock worse"

**Reproduced:** Placed an order and then cancelled it. The stock decreased after placing the order, but after cancellation it decreased again instead of returning to the original value.

**Cause:** The `releaseStock()` function was subtracting the cancelled quantity from the current stock instead of adding it back. it should be ' 'and not '-'
**Fix:** Changed the stock calculation from subtracting the quantity to adding the quantity back when an order is cancelled.

**Checked:** Checked the stock before placing the order, after placing the order, and after cancelling it. The stock returned to the original value after cancellation.

**Time:** about 15 mins in identifying the stock release logic and testing the fix


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
