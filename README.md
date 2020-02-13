# urinalysis-app
Prototype app to interpret urinalysis dipstick 

# background
I conceived of using a mobile phone to interpret urinalysis dipsticks while doing an away rotation in Ghana during medical school. It occured to me that there is significant inter-observer variability in performing and interpreting urinalysis dipstick results, which greatly limits the utility of the test. Using a smartphone camera to interpret the strip could standardize interpretation (improving accuracy) and provide a mechanism for documenting the observed results. Although resources are limited, smartphones equipped with cameras and urinalysis dipsticks are widely available even in low and middle income countries. In developing and developed countries alike, there are also significant errors in interpreting the results of urine dipstick tests, particularly when the results of each component are not considered together. Therefore, a smartphone app that used the phones camera for acquistion/interpretation of urine dipstick results could also be useful in clinics and EDs worldwide. An app would also potentially be useful for patients to test themselves or thier loved ones.


![test strip example](https://github.com/nickmmark/urinalysis-app/blob/master/figures/strip_interpretation.png)

Urinalysis test strips look like this:
![MultiStix interpretation](https://github.com/nickmmark/urinalysis-app/blob/master/figures/Bayer_MultiStix_interpretation.jpg)

They are interpreted using a schema such as this:

Test | Interpretation Time | Result Interpretation
------------ | ------------- | -------------
Leukocytes | 120 seconds | white == negative, purple == positive
Nitrite | 60 seconds | white == negative, light pink == positive
Urobilinogen | 60 seconds | light pink to dark pink <> 0.2 to 8 mg/ml
Protein | 60 seconds | light green == trace, green to dark green <> 1+ to 4+ protein
pH | 60 seconds | orange to green <> 5.0 to 8.0
Blood | 60 seconds | yellow w/ green spots to green <> trace to 3+ blood
Specific Gravity | 45 seconds | dark green to dark yellow <> 1.000 to 1.030
Ketone | 40 seconds | light pink to dark pink <> trace to 3+ ketones
Bilirubin | 30 seconds | white to grey/pink <> trace to 3+
Glucose | 30 seconds | blue to green to brown <> 0 to 2000 mg/ml glucose

Immediately, several challenges are evident:
- different samples require different amounts before they can be interpreted; reading too soon or too late can cause errors
- aligning the sample (which is covered in urine) to the guide (on the side of the bottle) is necessary to interpret the results; this can be messy and it is easy to misread ('frameshift error')
- there can be significant subjectivity in interpreting the results; [8% of men and 0.5% of women are color blind](https://en.wikipedia.org/wiki/Color_blindness)
- interpretation is sensitive to lighting conditions 
- the results must be promptly written down to document them before the strip changes (over-development)

# app design


# packages/libraries


# version history/known issues
v0.1.0 this is a work-in-progress

# license
open-source

# references
Simmerville JA et al, [Urinalysis: A Comprehensive Review](https://www.aafp.org/afp/2005/0315/p1153.html), Am Fam Physician. 2005
https://www.ncbi.nlm.nih.gov/pubmed/15125171
