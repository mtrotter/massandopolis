
My attempts to find what - if anything - is wrong with healthcare in Massandopolis, I focussed most of my energies on understanding the people of Massandopolis.

## Basic data quality assessment: 

Fairly complete. A few nulls here and there. One person who dies in the future. One annoying table join (see section on drugs below).

## Data analysis:

Since the question was phrased as "IS" wrong, I tried to focus on the last 20-30 years of data, even more recent in places. 


### Life and Death Stats

First, I checked out basic demographics. Ages, ages at death, base mortality rates, etc. It's clear mortality has been rising steadily, and the population is shrinking - there's no wonder the Massandopolans are worried.

At first I thought the increase in mortality rates could be just a function of an aging population, and certainly there's a bit of that there. 

There has been a big die-off of folks (especially men) born between 1929-1935, even since 2010, though the cause of death data isn't that suspicious. They do seem to have a fair big of lung troubles. A lot of natural causes, pneumonia and such. And they're the right ages to have worked in the famed Massandopolis coal mines) and likely smoke.

There's a hint of too-much-dying in the hispanic population, but I'd need more time/data to be sure.

My biggest worry about the deaths in Massandopolis are their causes. Drug overdose - even among the seniors - is a huge problem. 5% of senior deaths due to overdose? 50% of young-adult deaths? That's huge. 

### Drug problems

According to my ('codone') checks, 60% of all living Massandopoleans in the system have had a drug overdose. 45% have at least prescription for a drug with "codone" in the name - my lazy way of finding opioids (since the concept table had no obvious join). 

2268 living folk have had opioid prescriptions. Since 1990, Docs have written 8111 scripts for 'codone's. The medication - encounter - join I tried led to the "PROVIDER" column being the organization - not the actual prescribing doctor. So I couldn't nail down any individual over-prescribers. That information (prescribing doc) would have been very handy.

The hospitals where prescriptions are coming from I can't say are suspicious or not. However, the overabundance of encounters and condition-entries for "chronic pain" and "migraines" makes me wonder if we don't have some people blatantly drug-seeking and successfully.

Other common encounter reason-types - pregnancy, hyperlipidemia, CHF, viral sinusitis (cold), seem normal enough. 

I didn't see any obvious problems with drug costing, but would like to look more closely.

### Out of control diabetes

I had trouble finding diabetes encounters, and only 100 patients had medication entries for insulin. That would mean up to half the diabetics aren't getting insulin? Given the BMI distribution (30% obese or more) I would have expected more diabetes and more insulin. These patients may be being underserved, or refusing treatment. Either way, it doesn't look good.

## Out of time

I ran out of time for digging far into procedures, immunizations, imaging (lots of thoracic stuff - coal mines?) and care plans. I also didn't use the 'concepts' table to join anywhere because the other tables had "CODE" columns but not a code type - leaving it open to collisions. If it were me, I'd want code type specified in any table that uses "CODE".



## The notebook contains stream of consciousness evidence gathering and notes :)







