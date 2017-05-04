# GermEval2017
Use this script to check the format of your submission file and determine the performance w.r.t a gold labels file (e.g. on a  held out portion of the training data to gauge your system's performance).

How to use the script?
The  executable jar can be used to evaluate all subtasks (relevance, sentiment, category and OTE) and both tsv and xml submissions.
Run the executable jar using " java -jar EvaluationScript.jar relevance GOLDLABEL.xml YOUR_PREDICTION.xml " if you want to evaluate xmls. and " java -jar EvaluationScript.jar relevance GOLDLABEL.tsv YOUR_PREDICTION.tsv " 
Instead of of "relevance" type  sentiment, category or OTE to evaluate these attributes.

How to compile?
Although the script is built in java and therefore platform independent, you may want to build your own executable jar from the sources. This can be done with maven ("mvn clean install"). If you want to change java compatibility of the jar, alter the version specified in the maven compiler plugin to your preferred java version. The sources have been tested for java 7 and 8 (we use 7 in the current version).
