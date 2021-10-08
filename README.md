# segmented-pali
Segmented files for pali. These are the input files for the Buddhanexus neural network.

## Sources:

The Pāli textual corpus used in BuddhaNexus was obtained from the Mahāsaṅgīti Tipiṭaka Buddhavasse 2500: World Tipiṭaka Edition in Roman Script. Edited and published by The M.L. Maniratana Bunnag Dhamma Society Fund, 2005. Based on the digital edition of the Chaṭṭha Saṅgāyana published by the Vipassana Research Institute (VRI), with corrections and proofreading by the Dhamma Society.

The texts of the Suttas, Vinaya and Abhidhamma have been sourced from the SuttaCentral JSON-based segmented texts, which have been extensively tested to ensure integrity and correctness. These texts have the same segment numbers as in SuttaCentral and are linked to the corresponding segments on that site in table-view and numbers-view mode.

The remaining commentary texts of the Aṭṭhakathā, Tikā and Anya have been sourced from the Chaṭṭha Saṅgāyana as published by the Vipassana Research Institute.

For the calculation of the Pāli matches, SuttaCentral's hyphenation and stemming algorithms have been used.

### Types of input files:

The folder `inputfiles` holds the files with their original segmentation, including longer segments with multiple sentences.
The folder `inputfiles_cut_segments_for_TML_v2` holds the files with longer segments cut according to `.`, `?`, `;` and `:` so as to make them usable for the TML automated pali --> english translations.
The folder `inputfiles_cut_segments_for_NN` holds the files where longer segments are cut down even further, breaking on `,` as well. For the calculation of matches, smaller segments are preferable.

### Output files

Outputfiles match the inputfiles numbering for the TML.

Version 1 was a first try that had limited training data from SuttaCentral only. Version 2 also used training data from other sources.

In Version 2 (v2) there are two types of output files. Those marked with `44` was trained for 44900 epochs and `89` was trained for 89000 epochs. The actual output-files used for the BN website is a combination of the two.

It was found that 44900 epochs had less overfitting in files for which there had been no previous training data available. Files that have previously been translated by a human with the exact same segments did better with the 89000 epochs.

Therefore the first 4 Nikayas and part of the Khuddaka Nikaya use the output data after 89000 epochs as well as several other files that were used in the training.

Training data can be found in the buddhanexus/aligned_corpora repository.


