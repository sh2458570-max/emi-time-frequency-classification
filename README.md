# emi-time-frequency-classification
Course project on electromagnetic interference classification using STFT spectrograms, with robustness tests and filtering analysis.
# Time–Frequency Analysis and Classification of Electromagnetic Interference

**Author:** Xiaoyu Shang · Lisbon College, Shanghai University  
**Course project** · May–June 2026

[Read the full project report (PDF)](./Xiaoyu_Shang_EMI_Classification_Report.pdf)

## Research question

How does the choice of signal representation affect electromagnetic
interference (EMI) classification, and how well does the classifier
perform when signal conditions change?

## Experiments and findings

- Generated 1,500 simulated signals across five classes: normal operation,
  harmonic interference, broadband noise, impulse interference, and mixed interference.
- Compared time-domain waveforms, FFT spectra, and STFT spectrograms.
  STFT features gave the best results. Both SVM and CNN achieved 100% accuracy
  on the standard simulated test set.
- Tested the CNN under changes in noise, frequency, interference amplitude,
  and impulse strength. Accuracy dropped to 85.4% under the combined
  extreme-stress condition.
- Evaluated filtering on a representative harmonic-interference signal.
  Its severity score decreased from 0.256 before filtering to 0.000 afterward.

The experiments use simulated signals. Validation on measured EMI data
is a next step.
