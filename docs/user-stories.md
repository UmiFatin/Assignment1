# User Stories

Format: As a [type of user], I want [goal], so that [reason or benefit].

1. As a professional event photographer, I want to calculate a percentage score for each photo based on how many faces pass the eye, mouth, and head-pose checks, so that I can quickly identify the best group shots without manually checking every single face. (FR5)
   Acceptance criteria:
   - Given a photo with 5 detected faces, if 4 faces pass all checks and 1 face is blinking, the system displays a score of 80%.
   - If no faces are detected, the system displays a score of 0%.

2. As a photographer, I want to automatically categorize my photos into tiers (Good, Fair, Poor) based on their percentage scores, so that I can prioritize my editing workflow and focus only on the highest-quality images first. (FR6)
   Acceptance criteria:
   - Photos that achieve a score of 90% or higher are placed in the "Good" category.
   - Photos that score between 70% and 89% are placed in the "Fair" category, while scores below 70% go to the "Poor" category.

3. As a photographer, I want to check if the subjects' heads are facing forward, so that I don't have to manually delete photos where people are looking away or distracted. (FR4)
   Acceptance criteria:
   - If a subject's head is turned more than 30 degrees to the left or right, that specific face fails the check.
   - The system only analyzes the geometry of the face and does not attempt to recognize the identity of the person.
