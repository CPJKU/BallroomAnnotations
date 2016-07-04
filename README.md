Ballroom beat and bar annotations
===========

Description
------------
This data set includes `beat` and `bar` annotations of the ballroom dataset, introduced by Gouyon et al. [1]. It does not include the audio files. The audio files (698 files, size 1.5 gb) can be downloaded from:  
<http://mtg.upf.edu/ismir2004/contest/tempoContest/node5.html> (accessed latest Dec 2013).   
Md5sum of the file data1.tar.gz: 2872a3e52070bc342a4510a95e2fa0b8

Note: According to Bob Sturm (<http://media.aau.dk/null_space_pursuits/2014/01/ballroom-dataset.html>) there are four exact and nine recording replicas within the dataset. These include:

####Exact replicas

    Quickstep/Albums-AnaBelen_Veneo-11.wav matches Quickstep/Albums-Chrisanne2-12.wav      
    ChaChaCha/Albums-Fire-08.wav matches Samba/Albums-Fire-09.wav      
    ChaChaCha/Albums-Latin_Jam2-05.wav matches ChaChaCha/Albums-Latin_Jam2-13.wav      
    Waltz/Albums-Secret_Garden-01.wav matches Waltz/Media-104705.wav
    
####Recording replicas

    Rumba-international/Albums-AnaBelen_Veneo-03.wav matches Rumba-international/Albums-AnaBelen_Veneo-15.wav      
    Waltz/Albums-Ballroom_Magic-03.wav matches Waltz/Albums-Ballroom_Magic-18.wav      
    ChaChaCha/Albums-Latin_Jam-04.wav matches ChaChaCha/Albums-Latin_Jam-13.wav      
    Rumba-international/Albums-Latin_Jam-08.wav matches Rumba-international/Albums-Latin_Jam-14.wav      
    Samba/Albums-Latin_Jam-06.wav matches Samba/Albums-Latin_Jam-15.wav      
    Samba/Albums-Latin_Jam2-02.wav matches Samba/Albums-Latin_Jam2-14.wav  
    Rumba-international/Albums-Latin_Jam2-07.wav matches Rumba-international/Albums-Latin_Jam2-15.wav      
    ChaChaCha/Albums-Latin_Jam3-02.wav matches ChaChaCha/Media-103414.wav      
    ChaChaCha/Media-103402.wav matches ChaChaCha/Media-103415.wav




Format
------------
The annotations consist of `.beats` files that contain the beat and bar annotations in the following format:  
`beat time in sec` `beat id`  
E.g., 9.430022675	3  
means the third beat of a bar is located at 9.43 seconds. If you are looking for downbeats, extract all beats with id = 1.



   
Annotation strategy
------------
It is a well known problem that annotators disagree on the metrical level of a musical piece. In this dataset we relied on the tempo restrictions that are given by the dance style label of the ballroom dances. We therefore chose the metrical level of the beats according to the tempo ranges taken from:  
<http://www.ballroomdancers.com/Dances/>

Intros that do not contain any musical content have not been annotated, and should not be taken into account in the evaluation. The dataset was annotated using two stages: First, we used a beat tracker [2] to interpolate the (manual) bar annotations kindly provided by Simon Dixon and used in [3]. Then, we manually adjusted and corrected the interpolated beat times.

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


References
------------
[1] Gouyon F., A. Klapuri, S. Dixon, M. Alonso, G. Tzanetakis, C. Uhle, and P.
Cano. An experimental comparison of audio tempo induction
algorithms. Transactions on Audio, Speech and Language Processing
14(5), pp.1832-1844, 2006.  
[2] Böck, S., and M. Schedl. Enhanced beat tracking with context-aware neural networks. In Proceedings of the International Conference on Digital Audio Effects (DAFX), 2010.  
[3] Dixon, S., F. Gouyon & G. Widmer. Towards Characterisation of Music via Rhythmic Patterns. In Proceedings of the 5th International Society for Music Information Retrieval Conference (ISMIR). 2004.

If you use these annotations we are happy if you cite the following paper:    

  
F. Krebs, S. Böck, and G. Widmer. Rhythmic Pattern Modeling for Beat and Downbeat Tracking in Musical Audio. Proceedings of the 14th International Society for Music Information Retrieval Conference (ISMIR), Curitiba, Brazil, 2013.  
