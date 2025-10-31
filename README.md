Pns and ebs , 

Lettrage and ACT,  accounting and balancing automation


ebs is basically transaction that never matched in previous month (March)

Pns is daily transaction which have some groups and have a few matches already within a month. (April)

So 3 possible matches
- within pns itself when you do groupby it should basically already match the amounts , there might be few groups unmatched still (April)
- ⁠within grouping pns and ebs and joining them together you might match the unmatched in previous step but still have a few remaining (March -april)
- ⁠the few remaining would basically be ebs of the latest month and if you find which transaction these it should mostly match with the ebs file you have , these could basically be future transactions or installments that need to made . Can be verified by cross checking the april ebs file with our current excercise for previous month ( after everything remain is April unmatched ebs)
So for April the matching rate was around 66% = total transactions matched / total transactions

Then basically for the matched transactions , what we needed to do was basically find the positive and negative key mapping for each group 

Within the matched data, we basically just group by some other things do some distinct and to create positive transaction
And negative transaction tables
Then after doing that we join between both or merge 
And distinct to only get the final positive negative mapping and negative positive mapping
Then just basically concat them
The final key binding mapping is around 9k