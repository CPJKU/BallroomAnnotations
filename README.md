ballroom_db
===========

Description
------------
This data set includes `beat` and `bar` annotations which can be used for the evaluation of
beat and downbeat detection algorithms. It does not include the audio files. The audio files (size 1.5 gb) can be downloaded from:

<http://www.iua.upf.edu/mtg/ismir2004/contest/tempoContest/data1.tar.gz> (accessed latest Dec 2013). 
md5sum of the file data1.tar.gz: 2872a3e52070bc342a4510a95e2fa0b8

Format
------------
The annotations consist of `.beats` files that contain the beat and bar annotations in the following format:
<beat time in sec> <bar number>.<beat position within the bar>

E.g., 
9.430022675	9.3
means the third beat of the ninth bar is located at 9.43 seconds.

Reference
------------
If you use these annotations please cite the following paper:

F. Krebs, S. Böck, and G. Widmer.
Proceedings of the 14th International Society for Music Information Retrieval
Conference (ISMIR), Curitiba, Brazil, 2013.
   
Annotation strategy
------------
It is a well known problem that annotators disagree on the metrical level of a musical piece. In this dataset we relied on the tempo restrictions that are given by the dance style label of the ballroom dances. We therefore chose the metrical level of the beats according to the tempo ranges taken from:
<http://www.ballroomdancers.com/Dances/>

Intros that do not contain any musical content have not been annotated, and should not be taken into account in the evaluation.

Whenever we find errors in the annotations (I am sure there are still some!), we will create a new tag in the git repo and commit the changes. For any errors that you find, please contact Florian Krebs.

Contact: 
------------
Please send comments or errors that have been found in the annotations to
Florian Krebs <florian.krebs@jku.at>.

Acknowledgements
------------
We would like to thank Simon Dixon who supplied us with his annotations of the first bar of each piece.
