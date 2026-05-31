# 31/05 not forgeting to update the doc
- internet isnt interneting
- found a soloution for video + squares and stuff i just realized a important step the test data :)
- note to self if you are working on a serious project make stress test data first.
- found some words for it (Stress testing - Edge case testing - Robustness testing - Adversarial testing)
```
Tier 1 — Baseline (should work easily)
- 1.1 Direct camera, clean image in DB — same lighting, same angle
- 1.2 Direct camera, DB image from a different day (slight variation)

Tier 2 — Appearance Changes
- 2.1 Hat on
- 2.2 Glasses on (regular)
- 2.3 Sunglasses on
- 2.4 Mask on (partial face)
- 2.5 Beard / no beard (if applicable)
- 2.6 Different hairstyle or hair color

Tier 3 — Lighting Conditions
- 3.1 Bright direct light (overexposed)
- 3.2 Low light / dim room
- 3.3 Side lighting (strong shadow on half the face)
- 3.4 Backlit (face in shadow, bright background)

Tier 4 — Angle & Distance
- 4.1 Profile / side view (~90°)
- 4.2 Looking down or up
- 4.3 Far from camera (small face in frame)
- 4.4 Very close / large face in frame

Tier 5 — Motion & Video Quality
- 5.1 Walking past the camera
- 5.2 Motion blur
- 5.3 Low resolution video
- 5.4 Multiple people in frame simultaneously

Tier 6 — Adversarial / Edge Cases
- 6.1 Twin or very similar-looking people
- 6.2 Photo of a photo (printed face held up to camera)
- 6.3 Face partially occluded (hand, object)
- 6.4 Extreme emotion (mouth wide open, squinting)

What to track per test:
- Detected? (yes/no)
- Correct name? (yes/no/unknown)
- Confidence score (cosine similarity value)
- Notes (e.g., "detected but wrong name at 0.38")
```


---

# 23/05 intresting update 

1. (face detection on images)so there is a working version ( working is a genrous stand here ) on colab based on this vid with some updates (probably should post it here) : https://www.youtube.com/watch?si=EWGNIDw0W5Qvs5cQ&v=Y0dLgtF4IHM&feature=youtu.be

2. also working on a version that works on the video, percisly on cctv some good refrence : https://youtu.be/ppr_IOX2KSM?si=BFynuXW3P9LXtiZK

   
---

# 19/05 new tihs
- google colab is needed, or thousonds days of pain and misory is all upon us.
- fuck a|j.
- youtube better source than a terebite ai model :| .
- feeling sour af need cofee </3

---

# 18/05
starting from the open source projects https://github.com/deepinsight/insightface seems to have the most accurate models.
some importent and related links :
https://www.insightface.ai/solutions/face-recognition-licensing (for face recognition part of project)

## big mistake 
we should be race specific meaning cant put a model that is trained on western trained faces to work on middle eastern faces so we move toward an better model

## context summary so far

I'm building a local facial recognition system to identify people from photos by matching against a database of known faces. Priority is accuracy for Middle Eastern/Iranian faces.

Goal: Working system where, i connect this to an camer and can see who is passing it, identifying some stuff like mode name and... add this image to a database for further studies and evaluation.
