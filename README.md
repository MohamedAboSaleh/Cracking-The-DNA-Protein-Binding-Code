# Cracking-The-DNA-Protein-Binding-Code
This research delves into the mechanisms behind the process of DNA-binding proteins
(DBPs) locating their target sites within the genome. Despite a significant amount of
research in this area, there is still debate about how DBPs are able to quickly locate their
target sites. This study proposes a new hypothesis that certain nucleotide sequences in
DNA act as "pointers" that direct DBPs to the appropriate binding sites.
In our project we created a tool for finding the best candidates for such “pointers” by
different approaches. We also tested our algorithm for this goal. This algorithm iterates
through the DNA sequence using a sliding window of size k, moving the window one
position at a time. saving all unique combinations obtained during this process, and
analyzing them based on the properties of the pointers. The properties include different
occurrences in downstream and upstream regions, in the main and complementary
DNA strand, the asymmetry of the pointer pattern and other.
In the project implementation we met a difficulty with accessibility of the scientific data
concerning the in vivo occupied protein binding sites. It caused a significant delay and
only a part of the planned methods were applied. However, a clear signal in biological
sequence was detected, significantly stronger than in corresponding shuffled data. The
biological meaning of the discovered signal required additional investigation.
