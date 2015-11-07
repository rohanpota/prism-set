# The content of the PRISM set #

## Paper ##
prism\_evalset.pdf: paper describing the database in detail along with results obtained by running an iVector/PLDA MFCC system on the different conditions in the evalset.

## Keys ##
KEYS: directory with a file for each database containing the information described in the paper.
> The directory includes a file with the description of the fields in each of these files
> MIXxx refers to data from Mixer collection used for NIST SRE 20xx (not to the Mixer
> release itself). Below is a list of LDC links for each database:

> FISHATD5  http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC2006S29

> FISHE1    http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC2004S13

> FISHE2    http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC2005S13

> MIX10     not released yet

> MIX08     http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC2011S08
> > http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC2011S05
> > http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC2011S07


> MIX06     http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC2011S09

> MIX05     http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC2011S04
> > http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC2011S01


> MIX04     http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC2006S44

> SWCELLP1  http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC2001S13

> SWCELLP2  http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC2004S07

> SWPH1     http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC98S75

> SWPH2     http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC99S79

> SWPH3     http://www.ldc.upenn.edu/Catalog/CatalogEntry.jsp?catalogId=LDC2002S06


## TRIALS ##
directory containing, for each set X described in the paper, the following info:

  * X.sessions.G.{trn,tst}_list: enrollment and test lists (in many cases these two coincide) for each gender G
  * X.conditions: directory containing the list of trials for each gender for each condition within the set (as described in the paper).
> > Conditions are named with a prefix corresponding to the type of variability for which they are designed to assess the effect of, followed by a name
> > for the enrollment and test characteristics and the gender. The prefixes are the same as the set names in all cases except for set sch which is
> > divided in two: sty for assessment of style effects and chn for assessment of channel effects.
> > The enrollment and test characteristics for sets lan, sch and vel are described using four values:
> > tel or int: telephone conversation or interview
> > > phn, mic, mxx, myy: phn stands for telephone channel, mic for a generic microphone channel, mxx for one particular microphone channel,
> > > > myy for another microphone channel. Hence, mxx vs mxx condition is the "same mic" condition, while mxx vs myy is
> > > > the different mic condition. Note that same-mic trials include trials across mix08 and mix10. Two mics called the same
> > > > way across these two databases are supposed to be similar, but might not be identical and might be placed at different
> > > > distance to the subjects. For a stricter definition of same-mic trials, one could select only trials involving mix10 sessions.

> > > nml, hgh, low: vocal effort level
> > > eng, arb, tha, rus, chn, nat, lan, oth: for English, Arabic, Thai, Russian and Chinese and native English. lan stands for any particular
> > > > language so that lan vs lan trials correspond to same-language trials. oth stands for any language except English.

> > > Finally, for the vel and sch sets, additional conditions matching the sre10 conditions (but discarding held-out speakers) are created._

**LISTS: directory containing different session lists**

  * sessions\_from\_heldout\_speakers: All sessions from speakers not used in any of the trial sets above.
  * sessions\_from\_heldout\_speakers\_no\_rep: Subset of the list above discarding sessions that correspond to the same recording session but coming from different

> > databases, or of different lengths, etc.
> > These lists are the biggest possible set of sessions available for training the system.
> > Both lists include training sessions for the reverb and noise conditions. As the paper explains, these sessions are created using different reverb specification
> > and different noises than those used in the trials.

**NOISE: directory containing all the necessary information to create the noise signals used in the trials and the train lists. See the NOTES.NOISE for an explanation

> of how to create the noisy signals using the data in that directory.**

**REVERB: directory containing all the necessary information to create the reverberated signals used in the trials and the train lists. See the NOTES.REVERB for an explanation
> of how to create the reverberated signals using the data in that directory.**


Plans for future releases:

**A duration variability set is under design** We plan to eventually include a larger set of reverb types
**We plan to make both the SNR for noisy signals and the RT for reverberated signals**

If you are in need of any of these things, please ask us whether they are already in a state to be released.


Finally, if you find any issues with the current package (missing information, bugs, etc), please let us know even if you are able to fix it yourself. This way we can
improve the package in the next version.