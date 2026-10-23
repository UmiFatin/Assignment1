# Requirements

## Functional requirements (what the system must DO)
1. The system shall detect all human faces present in an uploaded photograph.
2. The system shall analyze detected faces using facial landmarks to determine if the eyes are open or closed.
3. The system shall analyze detected faces to determine if the mouth is open or closed.
4. The system shall The system shall estimate head pose to determine if the face is directed forward.
5. The system shall categorize each photo into tiers (Good ≥ 90%, Fair 70–89%, Poor < 70%) based on the calculated percentage.

## Non-functional requirements (how the system must PERFORM)
1. The system shall process and categorize a batch of 100 high-resolution images in under 60 seconds.
2. The system shall display the calculated percentage and category (Good/Fair/Poor) clearly on the user interface for each processed image within 1 second of processing completion.
3. The face detection module shall maintain an accuracy of at least 95% on standard frontal faces in well-lit conditions.
