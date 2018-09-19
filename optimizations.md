# Optimizations

## Where Do Learnings Take Place?

* Learning takes place at ad level, NOT ad set level. 
* Adset level learnings have some effect bunch are much less important
* **Learning means predicting click-through rate and post-click conversion rate.**
* Post-click conversion rate needs to be at the very least 0.5%, preferably over 1%.
* Each ad must have **25 lifetime conversions** for delivery optimization to work. 
* Each new ad  needs to run for 36 hours until learning takes effect

## What Will Reset Ad Learnings?

* Changing bid and budget is OK and will not reset learnings.
* Changing just about anything else \(title, message, photo, …\) will reset learnings because FB considers this to be a new ad. 
* If the ad goes to review process that will definitely mean that learning for that ad starts from scratch.

## Account level learnings

* Accounts also collect learnings \(used as priors for new ads\).
* It is not fair to compare performance against an existing account. All cross-account bake-offs MUST use new accounts.
* New accounts use country/objective level priors.

## Delivery issues

* Most common cause of delivery issues: 
  * CTR is low 
  * or CR is low
* What to do if you do not get delivery:
* * Massively increase bid \(or budget if the adset if budget limited\).
  * If using autobid increase budget.
  * Relaunching the ad might also help because there is some randomness in getting initial conversions.

## Deduping

* Deduplication happens also on object level \(page/app\).
* If another account shows ads for the same page, only one of the accounts will be able to show an ad for each user.
* This is why you absolutely must use an ad study with bake-offs

## AutoBid

* Autobid will keep increasing your bid so that the budget is spent; in theory it should always spend the entire budget.
* Bid can go up to 95th percentile of bids in country/objective; there is no fixed dollar cap otherwise.
* The bid distribution is not updated in real time, so when bids suddenly increase \(e.g. on Black Friday\) the cap might be much lower than 95th percentile and hence auto-bid fails to spend the budget.

## Fun Facts

* 25 conversions is enough to provide roughly 90% accuracy for predicting conversion rates.
* Facebook uses up to 90 days of user level data in optimization. This is based on EU regulations but the same 90 days is commonly used throughout Facebook.
* There is time decay for learning, so last days matter more. This also depends on the amount of data: if you spend over $10k per day and get tons of impressions then older data has less influence.

