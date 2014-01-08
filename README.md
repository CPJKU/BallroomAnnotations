Ballroom beat and bar annotations
===========

Description
------------
This data set includes `beat` and `bar` annotations of the ballroom dataset, introduced by Gouyon et al. [1]. It does not include the audio files. The audio files (698 files, size 1.5 gb) can be downloaded from:  
<http://mtg.upf.edu/ismir2004/contest/tempoContest/node5.html> (accessed latest Dec 2013).   
Md5sum of the file data1.tar.gz: 2872a3e52070bc342a4510a95e2fa0b8

Note: File `Albums-Latin_Jam-06` and `Albums-Latin_Jam-15` are identical.

[1] An experimental comparison of audio tempo induction
algorithms.
F. Gouyon, A. Klapuri, S. Dixon, M. Alonso, G. Tzanetakis, C. Uhle, and P.
Cano. IEEE Transactions on Audio, Speech and Language Processing
14(5), pp.1832-1844, 2006.


Format
------------
The annotations consist of `.beats` files that contain the beat and bar annotations in the following format:  
`beat time in sec` `bar number`.`beat position within the bar`  
E.g., 9.430022675	9.3  
means the third beat of the ninth bar is located at 9.43 seconds.

Reference
------------
If you use these annotations please cite the following paper:    

Rhythmic Pattern Modeling for Beat and Downbeat Tracking in Musical Audio  
F. Krebs, S. Böck, and G. Widmer. Proceedings of the 14th International Society for Music Information Retrieval Conference (ISMIR), Curitiba, Brazil, 2013.  
   
Annotation strategy
------------
It is a well known problem that annotators disagree on the metrical level of a musical piece. In this dataset we relied on the tempo restrictions that are given by the dance style label of the ballroom dances. We therefore chose the metrical level of the beats according to the tempo ranges taken from:  
<http://www.ballroomdancers.com/Dances/>

Intros that do not contain any musical content have not been annotated, and should not be taken into account in the evaluation.

Version control
------------
Note that the annotations are stored in a versioning system, which allows us to update the annotations from time to time while keeping track of older versions. Whenever new errors in the annotations are identified and resolved (I am sure there are still some), we will create a new tag in the git repo and commit the changes. In order to assure the reproducibility of your results, it would also be advisable to include the tags into your publications. 

Error reporting and contact
------------
We strongly encourage everybody to report errors in the dataset to  
Florian Krebs <florian.krebs@jku.at>. 

Acknowledgements
------------
We would like to thank Simon Dixon who supplied us with his annotations of the first bar of each piece.
