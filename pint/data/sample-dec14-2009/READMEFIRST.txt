This sample-dec14-2009 folder contains the following:

1. this READMEFIRST.txt file

2. resources folder
	2.1 examples.rdf
	2.2 RNRM.rdf
	2.3 signatures.rdf
	2.4 WTI.rdf
	
3. helper-files

	3.1 combined.csv
	3.2 groundtruth-recipe1.txt
	3.3 noise_key.csv
	3.4 samplecode.txt
	
4. observations.data

--

The observations.data file contains 5000 serialized SimpleObservation objects that correspond to the 5000 rows of observations in the combined.csv file.

The samplecode.txt contains a snippet that will read the content of observations.data.

The groundtruth-recipe1.txt file contains the list of observations that support a process. A process finder is expected to detect the process implied by the observables that are supported by these observations.

The noise_key.csv file contains the list of "confusers" in the observation data. They are not meant to support any processes. Although, by chance, it is possible that a collection of these observations may trigger a detection.

The observations.data and combined.csv files ALREADY contain data in the groundtruth-recip1.txt and noise_key.csv files.

The files in the resources folder contain knowledge of the model, and are required.
