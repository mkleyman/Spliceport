Readme for SpliceportScorer.jar and FeatureConverter.jar

SpliceScorer: Scores possible donor and acceptor sites in a provided fasta file based on how likely they are to be true splicing donor or acceptor sites. 
	Execution Command Sample: java -jar SpliceportScorer.jar -t 5 -f HPRT1.fasta -d donorFeatures.txt -a acceptorFeatures.txt -w 162
	Options:
	-w: Window Size
	-t: Number of Threads(optimally number of processors avialable +1, default is 2)*
	-f: Input Fasta File
	-a: Acceptor Feature File (Spliceport 2.0 feature file type)
	-d: Donor Feature File	(Spliceport 2.0 feature file type)
	-o: Output file 
	*Optional Argument
	
FeatureConverter: Converts Spliceport 1.0 feature files to Spliceport 2.0 feature files
	Execution Command Sample: java -jar FeatureConverter.jar -d donorFeatures.txt -a acceptorFeatures.txt -w 162 -od new_don.txt - oa new_acc.txt
	Options:
	-w: Window Size
	-a: Acceptor Feature File (Spliceport 1.0 feature file type)
	-d: Donor Feature File	(Spliceport 1.0 feature file type)
	-oa: Output Acceptor File (Spliceport 2.0 feature file type)
	-od: Output Acceptor File (Spliceport 2.0 feature file type)

	
