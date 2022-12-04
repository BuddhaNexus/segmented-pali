# segmented-pali
Segmented files for pali. These are the input files for the Buddhanexus neural network.

## Sources:

The Pāli textual corpus used in BuddhaNexus was obtained from the Mahāsaṅgīti Tipiṭaka Buddhavasse 2500: World Tipiṭaka Edition in Roman Script. Edited and published by The M.L. Maniratana Bunnag Dhamma Society Fund, 2005. Based on the digital edition of the Chaṭṭha Saṅgāyana published by the Vipassana Research Institute (VRI), with corrections and proofreading by the Dhamma Society.

The texts of the Suttas, Vinaya and Abhidhamma have been sourced from the SuttaCentral JSON-based segmented texts, which have been extensively tested to ensure integrity and correctness. These texts have the same segment numbers as in SuttaCentral and are linked to the corresponding segments on that site in table-view and numbers-view mode.

The remaining commentary texts of the Aṭṭhakathā, Tikā and Anya have been sourced from the Chaṭṭha Saṅgāyana as published by the Vipassana Research Institute.

For the calculation of the Pāli matches, SuttaCentral's hyphenation and stemming algorithms have been used.

### Types of input files:

The folder `inputfiles` holds the files with their original segmentation, including longer segments with multiple sentences.

Several files from SuttaCentral Bilara have been merged. This is the case for the AN, SN and DHP.

The folder `inputfiles_cut_segments_for_NN` holds the files with longer segments cut according to `.`, `?`, `;`, `:` and `,` so as to make them usable for the calculation of matches.




