README
Retention Probability (RPr) calculator
https://github.com/covert-koala/memory_retention/blob/master/RPr-calculator_protected.xlsx
https://github.com/covert-koala/memory_retention/blob/master/RPr-calculator_unlocked.xlsx


Please note:
1.	The locked version of the calculator is titled “RPr-calculator_protected.xlsx”.
2.	The unlocked version of the calculator is titled “RPr-calculator_unlocked.xlsx”.
3.	If you edit syntax on the unlocked version but later decide to use the original calculation, please refer to the locked version to ensure correct formula specification.


Calculator instructions:
Enter maximum possible initial recall score in green-highlighted cell. Enter initial and delayed recall score pairs in yellow-highlighted columns. Do not alter other cells (if using unlocked version, alter at own discretion). First row is an example. Table can be extended for more subjects by using the fill handle to populate formulae in cells below. α and β=alpha and beta parameters, respectively, of beta distribution. B(α,β)=beta function. E[q]=average value from distribution. σ[q]=standard deviation of distribution. RPr=retention probability. PR=percent retention (traditional method).

Example data from the Hopkins Verbal Learning Test-Revised (HVLT-R):
Generic formulas are included in the first example.

Person A:
Best performance of learning trials 2 or 3 = 12 words (“Initial recall” [IR])
Delayed recall (DR) = 12 words
α = DR + 1 = 12 + 1 = 13
β = 1 + IR - DR = 1 + 12 – 12 = 1
B(α, β) = (α - 1)! * (β - 1)! / ( α + β - 1)! = (13 - 1)! * (1 - 1)! / (13 + 1 - 1)! = .0769
E[q] = α / (α + β) = 13 / (13 + 1) = .9286
σ[q] = √(α * β / ((α + β)2 * (α + β +1))) = √(13 * 1 / ((13 + 1)2 * (13 + 1 +1))) = .0665
RPr = (E[q] / σ[q]) / 13.964 *100 = (.9286 / .0665) / 13.9642 *100 = 100
PR = DR/IR * 100 = 100

Person B:
IR=5, DR=5
α = 5 + 1 = 6
β = 1 + 5 – 5 = 1
B(α, β) = (6 - 1)! * (1 - 1)! / (6 + 1 - 1)! = .1667
E[q] = 6 / (6 + 1) = .8571
σ[q] = √(6 * 1 / ((6 + 1)2 * (6 + 1 +1))) = .1237
RPr = (.8571 / .1237) / 13.9642 *100 = 50
PR = 5/5 * 100 = 100

Person C:
IR=10, DR=9
α = 9 + 1 = 10
β = 1 + 10 – 9 = 2
B(α, β) = (10 - 1)! * (2 - 1)! / (10 + 2 - 1)! = .0091
E[q] = 10 / (10 + 2) = .8333
σ[q] = √(10 * 2 / ((10 + 2)2 * (10 + 2 +1))) = .1034
RPr = (.8333 / .1034) / 13.9642 *100 = 58
PR = 9/10 * 100 = 90

Rank ordering of subjects by PR:
1. A & B (tie; 100)
3. C (90)
Rank ordering of subjects by RPr:
1. A (100)
2. C (58)
3. B (50)

As shown, discrepancies in rank ordering of subjects between the two scoring procedures may occur due to differences in learning level. Person A performed at true ceiling. Person B had 100 PR, but only learned 5 words (pseudoceiling effect). Person C recorded a PR score below A and B, but RPr scores suggest that their performance is stronger than that of Person B because they learned considerably more words in addition to retaining a high percentage of these words.


