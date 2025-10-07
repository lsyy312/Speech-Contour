
# HW1 – Acoustic Feature Extraction

## How to run
1. Install dependencies:
   ```bash
   python -m pip install praat-parselmouth

2. Place your recordings in the same folder as the script:

   ```
   Happy.wav  Angry.wav  Sad.wav  Afraid.wav  Surprised.wav  Disgusted.wav  Neutral.wav
   ```
3. Run the extraction:

   ```bash
   python script.py
   ```

   The resulting CSV file will appear in the same directory with 12 feature columns following the provided template.

## Files

* **my_features.csv**, **msp_features.csv** — Feature tables matching the template.
* **script.py** — Python feature extraction script using Parselmouth.
  Extracts Pitch, Intensity, Jitter, Shimmer, HNR, and Speaking Rate.
  Speaking rate uses manual word counts defined in a filename mapping at the top of the script.
* **HW1_Report.pdf** - Text file with my responses to each question.
* **Happy.wav  Angry.wav  Sad.wav  Afraid.wav  Surprised.wav  Disgusted.wav  Neutral.wav** - My emotion recordings.
* **bonus1.Manipulation**, **bonus1.wav** — Manual manipulated sound.
* **bonus2.Manipulation**, **bonus2.wav** — Pitch contour cloned from the *Happy* recording.



## References

[1] P. Boersma and D. Weenink, Praat: Doing phonetics by computer, computer program, University of Amsterdam. [Online]. Available: https://www.praat.org

[2] Y. Jadoul, B. Thompson, and B. de Boer, “Introducing Parselmouth: A Python interface to Praat,” J. Phonetics, vol. 71, pp. 1–15, 2018. [Online]. Available: https://doi.org/10.1016/j.wocn.2018.07.001

[3] C. M. Lee and S. S. Narayanan, “Toward detecting emotions in spoken dialogs,” IEEE Trans. Speech Audio Process., vol. 13, no. 2, pp. 293–303, 2005. [Online]. Available: https://doi.org/10.1109/TSA.2004.838534


## Notes

* The script avoids using disallowed NumPy shortcut methods (e.g., no `to_feature()` calls).
* Word counts exclude filled pauses (“um”, “uh”) and repeated disfluencies (e.g., “I… I”).
* File names must exactly match the assignment template for correct feature extraction.

```
```
