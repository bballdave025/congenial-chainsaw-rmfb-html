# congenial-chainsaw-rmfb-html
~~HTML~~ Microsoft Word saved as PDF that exposes the XML used in the classifier, allowing the descriptions and examples to be more-easily seen. It will be a good guide for me to remember which things I want classified in which way (and thus to be consistent). It will also track the classification changes and addenda that always come with such classification projects

## Reused Manuscript Fragments in Bindings - for the short and not-quite-complete version.

~~Maybe I'll change the name to be more accurate.~~ The more accurate name, which is still not used as much as 
**R**eused 
**M**anuscript 
**F**ragments in 
**B**indings, 
(RMFB) is 
<strong>R</strong>eused <strong>I</strong>nformation <strong>B</strong>earing <strong>Wri</strong>ting <strong>S</strong>urface <strong>T</strong>races <strong>in</strong> <strong>Bin</strong>-<strong>Din</strong>-gs (rib-wrist-in-bin-din).

**Edit (2026-10-03)**: The short-form name has now been changed to RMMFB (pronounced R double-M F B,) for
**R**eused 
**M**anuscript and
**M**achine-created
**F**ragments in 
**B**indings, 

## A bit of vision

Taken from a Jupyter notebook,

https://colab.research.google.com/github/bballdave025/rib-wrist-in-bin-din/blob/main/Paper_Code_Prep_01.ipynb

whose housing repos are

https://github.com/bballdave025/rib-wrist-in-bin-din/tree/main

and

https://github.com/bballdave025/fhtw-paper-code-prep

Note that a (very drafty) draft, more of a directed steam of consciousness with vision, references, and ideas , is on my Google Drive at 

https://docs.google.com/document/d/1JAIL4PFmIm3_gScfscTj88yXKjorG7NIcXnTlT2IcSI/edit?usp=drivesdk

---

---

David BLACK, GitHub @bballdave025 ,

Working Title for Technical Paper: &quot;AI Computer Vision Methods for
Finding Information-bearing Writing Surfaces (Especially Codex Fragments) Reused in Other Codex Bindings&quot;

Working Title for <em>Fragmentology</em>
(Manuscript Studies) Paper: None Yet
(It would be nice to have some statistics.)

---

## Why these Notebooks/Drafts?

There are several reasons for writing these notebooks and doing these various visualizations. The most acceptable (I almost put that in quotation marks; I mean the most-what-employers-or-theoretical-AI/ML-people-would-like-to-hear) answers are: <br/>&nbsp;&nbsp;&nbsp;1) I want to give <strong>greater explainability of the CV model  decisions</strong>,  especially as it relates to the audience of the paper and their acceptance of a non-manual, non-human method, possibly seen as an intruder into the Manuscript Studies community. I think that if they see the model  making decisions in the same way that <em>they</em> would make decisions, they will be more likely to see it as an aide doing such things as allowing grad students to analyze fragments rather than finding them. For clarity, I mention that the audience consists of the readers of the Binding-Fragment paper to be submitted to <em>Fragmentology</em>; <br/>&nbsp;&nbsp;&nbsp;2) I want to make better decisions as to which model will most-likely make the <strong>goal of ~95% precision and ~70% recall possible on a wide variety of writing-material and binding images</strong>. The ultimate goal for (this stage of) the study is to run the algorithm over as many of FamilySearch's earliest-to-18th Century images (let's make it readable: images from the earliest records they have up to the 1700s) as possible. Through the analysis and visualization of how well the chosen model or models performs, we can have higher confidence that an eventual <strong>one run</strong> over what I'll estimate as 0.5 to 1 billion images with a thoroughly tested and understood/explainable model will <strong>suffice for at least a decade</strong>. <br/>&nbsp;&nbsp;&nbsp;3) (This is a long one.) Especially with the Grad-CAM visualizations of the salient features for model decisions, I want to have something to <strong>show to the Manuscript Studies/Fragmentology community that will get them excited</strong> about <em>helping us</em> to <em>create better training sets</em> and to <em>help create new training sets for interesting phenomena/occurences</em> (for lack of a better word describing what each of the classifications describes). I think that the best example of this is to create a model (or add to the existing model) the search for images that not only have iron-gall-ink damage to the point of going through the page (something I have tried to do without expertise), but which are at different stages<sup>\[NB5\]</sup> of the iron-gall-ink (and other corrosive dye) damage process. I'm also going to face the fact that, even as concerns the main object of study—fragments found in bindings—I'm perhaps passingly knowledgeable but by no means an expert. Seeing heat maps describing what the model thinks is most important in finding a specific images I've classified should make this a more interesting invitation, as it allows quick view of the types of phenomena such models can find in and on writing materials, bindings, etc.

For my estimate of the sum total of such documents, I make reference to the <em>Company Facts</em> page on FamilySearch [as I see it now (archived with numbers updated 2025-04-07)](https://web.archive.org/web/20250423044740/https://www.familysearch.org/en/newsroom/company-facts), which reports "5.65 Billion \[Digital Images Published\]" . For a second opinion, I've looked at the running counter of images digitized at https://www.familysearch.org/en/records/images/, which is at \[let me go take a screenshot\]

<br/>
<div>
  <img src="https://raw.githubusercontent.com/bballdave025/rib-wrist-in-bin-din/refs/heads/main/FamilySearch_5667347462_5point667-B_Images_2025-04-22T113500-0600.png"
       alt="Screenshot of family search dot org forward slash E N forward slash records forward slash images. Tab name is. QUOTE. Explore Historical Images. END QUOTE. Visible text is. QUOTE. Access billions of documents newline FamilySearch has been collecting historical documents since eighteen ninety four and currently has. Left square bracket. Transcriber's note colon. Number in short scale, i.e. without milliard, billiard, et cetera, so ten to the ninth is read billion, ten to the twelfth is read trillion, et cetera. Right bracket. five billion six hundred sixty-seven million, three hundred forty-seven thousand four hundred sixty-one images from all over the world. That makes FamilySearch one of the world's largest collections of historical documents exclamation point. END QUOTE. Bottom toolbar shows eleven colon thirty-five A M. and. four slash twenty-two forward slash two thousand twenty-five. Left Bracket. Date format is as in the stupid U S A format comma month slash day slash year. Right Bracket. An errow points from the annotated text. QUOTE. M D T. Left parenthesis. G M T minus six Right parenthesis. END QUOTE. to the time and date."
       width="500px">
</div>
<br/>

5,667,347,461 (five billion six hundred sixty-seven million, three hundred forty-seven thousand four hundred sixty-one) images. The type of binding we're seeking is most-commonly found in Western and Central Europe going into Russia and Persia, with some around the Mediterranean—including Muslim and Jewish records—the Near East, and the Americas—mostly (Catholic) South America. Since I think that records from the current United States of America probably take up at least a third of all digital images published, and Western/Central Europe <em>at least</em> one quarter of the remaining digital images, my guess is that a search in those geographical regions from the earliest date for which FamilySearch has records to 1799 will yield approximately<br/>$ \frac{2}{3} \cdot \frac{1}{4} \cdot 5.66 \times 10^{9} $ images or $ 9.45 \times 10^{8} \left(\substack{+9e8 \\ -5e9} \: \mathrm{systematic}\right) \left(\pm 0.25e9 \;  \mathrm{who} \! \cdot \! \mathrm{knows}\right) $,<br/>$ \frac{1}{6}\;\mathrm{ish} $ of the records, 500 million to 1.5 billion (again, very $ \mathrm{-ish} $).<br/>(Note that my methodology will let in records from the 1800s and even a few from the 1900s, but not on purpose.)

The current study will include around hundreds of thousands of images, with an approximate guess of half being from FamilySearch, for the intial study and publication in <em>Fragmentology</em>. This study entails at least thousands of images, up to tens of thousands, for the training, validation, and test sets. (That is, tens of thousands of images split into the three sets.)

---

#### More Notes

Blank space for notes



---

---

## Short view of classifications

### Smallest Classification Instructions — (Readable / Printable)

| c? | Classification Directory Name | Kbd 1 lett | 3 letters | Any Mnemonic Explanation | Shows Up As |
|---|---|---|---|---|---|
| c1 | Outside_Cover_Reuse | O | orc | Don't want to confuse optical character recognition, so outside reuse cover | Outside cover reuse |
| c2 | Under_Cover_Reuse | R | ucr | Initialism | undeR coveR reuse |
| c3 | Spine_Protection_Reuse | P | spr | Initialism | sPine Protection reuse |
| c4 | Front-back_Matter_Reuse | F | fmr | front matter reuse | Front-back matter reuse |
| c5 | One_Behind_Reuse  \nN.B. Won't be 'H' | H | obr | Initialism  \nTRYING WITHOUT THIS FOR FHTW 2025 | one beHind reuse |
| c6 | Cover_Wraparound_Reuse | W | cwa | cover wraparound cover | Wraparound reuse |
| c7 | Tiny_Background_Reuse | T | tbr | Initialism |  |
| c8 | Connecting_or_Guard_Reuse | C | scg | small connecting or guard | Connecting or guard reuse |
| c9 | Across_Book_Gutter_Reuse  \n(Note this includes across-book-gutter OIC; dir name to change after project) | G | abg | across book gutter | across book Gutter reuse |
| c10 | Wrapper_Reuse | 4 | wpr | wrapper | wrapper reuse (4) |
| c? | Classification Directory Name | Kbd 1 lett | 3 letters | Any Mnemonic Explanation | Shows Up As |
| %c11 | Not_In_Situ_Reuse_Cover | V | nsc | not in situ reuse cover | %%%% TO %%%% |
| %c12 | Not_In_Situ_Reuse_Front-back | A | nsf | not in situ reuse front-back | %%%% BE %%%% |
| %c13 | Not_In_Situ_Reuse_Spine_Protection | 9 | nsp | not in situ reuse (s)pine | %%% COMB- %% |
| %c14 | Not_In_Situ_Reuse_Small_Connecting_Guard | 7 | nst | not in situ reuse connecting like (s)trap; 7 like a backwards gamma -> G sound -> Guard | %%% INED %%%% |
| c15 | General_Not_In_Situ_Reuse | Y | gni | general not in situ reuse; Y as in whY are these so difficult? |  |
| ... | ... | ... | ... | Perhaps more, one day ... | ... |
| c101 | Multiple_Classes | = | mcl | multiple classes | multiple classes (=) |
| c102 | Multiple_Binding_Reuse_Classes | B | mbr | multiple binding reuse | multiple Binding reuse classes |
| c103 | Multiple_Mixed_But_All_Not_Binding | X | mmx | multiple mixed (the x can help you think of not binding; the word, binding, x-ed out) | multiple miXed but all not binding |
| ... | ... | ... | ... | Maybe multiple more, but idk. | ... |
| c? | Classification Directory Name | Kbd 1 lett | 3 letters | Any Mnemonic Explanation | Shows Up As |
| c111 | Fake_Out | K | fko | fake-out | faKe-out |
| c112 | Important_as_Counter_Example  \n(could also be called ... as contrast, often, has a structure that would be a class, but no information of the surface) | Z | iac |  |  |
| <sup>†</sup>~~c113~~ | <sup>†</sup>~~Somewhat_Uneasy_with_Classification_or_Hard  \n~~ ~~<sup>†</sup>[Initially considered Uneasy_with_Positive but decided wider class (possibly including negatives) with those I find or that I think the algorithm will find hard]~~\n<sup>†</sup>See description after the table, specifically _§More Notes, Edit (2026-10-03)_ | <sup>†</sup>~~H~~ | <sup>†</sup>~~suh~~ | <sup>†</sup>~~somewhat uneasy hard~~ | <sup>†</sup> |
| ... | ... | ... | ... | ... | ... |
| c121 | No_For_Binding_Reuse | 0 | nbr | no for-binding reuse | n0 for binding reuse (0) |
| c122 | No_Binding_Reuse_but_Other_Interesting_Classes | - | oic | other interesting classes | other interesting classes (-) |
| c123 | Nothing_Interesting | N | noi | nothing of interest | NothiNg iNterestiNg |
| c124 | Do_Not_Use | D | dnu | Initialism | Do not use |
| c125 | Unsure | U |  | no addition is given, so that when someone else checks the image, they can classify it however is needed | UnsUre |
| ... | ... | ... | ... | Likely not many (or none) after this. | ... |

**Notes:** Contains only the classes used for the fragments-in-bindings study for the Family History Technology Workshop in 2025. At the moment, I'm leaving the "one beHind reuse" class out of the FHTW 2025 parameter file, though that might change.

**More Notes, Edit (2026-10-03)**: The continuing studies after the inability to go to FHTW 2025 are using the same procedures as noted here, especially as work is done towards a submission to the 2026 [_Fragmentology_](https://www.fragmentology.ms/).

**†** Deprecated classification: `suh` (`c113`, _Somewhat_Uneasy_with_Classification_or_Hard_) is not part of the current RMMFB/Fragmentology-2026 (previously RMFB/FHTW2025) classification scheme. It had been omitted from the active FHTW2025 classification helper by 2025-03-01. Some historical filenames in the frozen 3,331-image corpus retain the `_suh` token; these filenames are preserved for provenance, and `suh` is ignored when deriving current labels. (Continuation of 2026-10-03 Notes)

### Other classes to be used later in Manuscript Studies things

| Possible number / Dir Name | three-letters |
|---|---|
| c50 / Stitching_Any_Type | stc |
| Should later be moved into one of the following three |  |
| c51 / Stitching_Level_1 | st1 |
| (parchment maker, basic repairs with twine, no-longer-there veil stitch holes, ... anything else I think of) |  |
| c52 / Stitching_Level_2 | st2 |
| (beyond basic twine, hole stitch, not embroidery, baseball stitch, green Vs, ... other things maybe) |  |
| c53 / Stitching_Level_3_Embroidery_etc | st3 |
| (Embroidery, in-place veils, other fancy, ... and blah and blah and blah) |  |
| c54 / Manicule | man |
| c55 / Non_Manicule_Nota_Bene | nmn |
| c56 / Fingerprint | fgp |
| (Has to have loops/whirls, or at least visual separation between the grooves ... any other details) |  |
| c57 / Hair_on_parchment | hop |
| (Meaning animal hair, like in the holes of the parchment, or even still looking like fur/wool on a used page) |  |
| c58 / Very_Visible_Watermark | vvw |
| c59 / Not_For_Binding_Reuse | nfb |
| c60 / Iron_Gall_or_other_Corrosion_Thru | igt |
| c61 / Squished_Bug_Remains | sbr |
| c62 / Alphabet_or_Pen_Trials_or_Counting | apc |

Other classification ideas, as well as more details about and several image examples for the main reuse document classifications are in the repo files

---
