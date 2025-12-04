## Assignment: Evaluating Fine-Tuned LLM Performance
Written by Bade Habib

### Task & Model Used
**Task:** Text Classification

**Model:** fine_tuned_bert_imdb

### Metrics
|Metric|Result|
|---|---|
|Accuracy|52.00%|
|Precision|50.00%|
|Recall|45.83%|
|F1 Score|0.47|

### Metric Justification
F1 Score is more useful than Accuracy when measuring successful prediction because data sets may not have balanced classifications between positive and negative results. In the case of this dataset, there were 22 positive classifications and 28 negative classifications. While Accuracy ends up being higher because overall there were more proper classifications, the F1 score ends up being lower because the score is measuring the number of false positives and false negatives compared to the total number of classifications in the dataset. In this case, the lower Recall value is not fully represented in the Accuracy value, whereas it is more properly represented in the F1 Score.

### Error Analysis
Recall was the worst performing metric at **45.83%**. The two cases below indicating false negatives are examined and analyzed.

#### **Case 1**
**Review:** When I unsuspectedly rented A Thousand Acres, I thought I was in for an entertaining King Lear story and of course Michelle Pfeiffer was in it, so what could go wrong? Very quickly, however, I realized that this story was about A Thousand Other Things besides just Acres. I started crying and couldn't stop until long after the movie ended. Thank you Jane, Laura and Jocelyn, for bringing us such a wonderfully subtle and compassionate movie! Thank you cast, for being involved and portraying the characters with such depth and gentleness! I recognized the Angry sister; the Runaway sister and the sister in Denial. I recognized the Abusive Husband and why he was there and then the Father, oh oh the Father... all superbly played. I also recognized myself and this movie was an eye-opener, a relief, a chance to face my OWN truth and finally doing something about it. I truly hope A Thousand Acres has had the same effect on some others out there. Since I didn't understand why the cover said the film was about sisters fighting over land -they weren't fighting each other at all- I watched it a second time. Then I was able to see that if one hadn't lived a similar story, one would easily miss the overwhelming undercurrent of dread and fear and the deep bond between the sisters that runs through it all. That is exactly the reason why people in general often overlook the truth about their neighbors for instance. But yet another reason why this movie is so perfect! I don't give a rat's ass (pardon my French) about to what extend the King Lear story is followed. All I know is that I can honestly say: this movie has changed my life. Keep up the good work guys, you CAN and DO make a difference.

**Analysis:** This misclassification was likely due to the many negative words (abuse, angry, denial) used in the review, creating ambiguity.

#### **Case 2**
**Review:** This is the latest entry in the long series of films with the French agent, O.S.S. 117 (the French answer to James Bond). The series was launched in the early 1950's, and spawned at least eight films (none of which was ever released in the U.S.). 'O.S.S.117:Cairo,Nest Of Spies' is a breezy little comedy that should not...repeat NOT, be taken too seriously. Our protagonist finds himself in the middle of a spy chase in Egypt (with Morroco doing stand in for Egypt) to find out about a long lost friend. What follows is the standard James Bond/Inspector Cloussou kind of antics. Although our man is something of an overt xenophobe,sexist,homophobe, it's treated as pure farce (as I said, don't take it too seriously). Although there is a bit of rough language & cartoon violence, it's basically okay for older kids (ages 12 & up). As previously stated in the subject line, just sit back,pass the popcorn & just enjoy.

**Analysis:** This misclassification was likely due to the reviewer pointing out problematic aspects of the film, creating ambiguity.
