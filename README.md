# Minimal Structural Reranking Pipeline

Thisi is a stripped down version of the reranking pipeline.  

With this software you will be able to apply structural reranking on a question answering dataset.

## Prerequisites

### UIMA

Go to https://uima.apache.org/downloads.cgi and download the latest binary distribution of UIMA.  

Decompress the archive and set the $UIMA_HOME environmental variable to the bin/ folder in the
UIMA distribution directory. You can use export="path/to/dir" if you use Linux/Mac and add this line
to ~/.bashrc in order to automatically set it in the future.

### Maven

You will need Maven for building this project. Install maven for your operating system (e.g. sudo
apt-get install maven).  

If you use Eclipse please install the M2E plugin. Go to Help > Install new software... and search
for m2e.

### UIMA tooling for Eclipse

UIMA tooling simplifies the development of typesystems and annotators in Eclipse. Install Eclipse EMF
following these instructions: http://tinyurl.com/UIMA4ECLIPSE. The useful UIMA visual
tools (UIMA tooling) can be found at this software update address:
http://www.apache.org/dist/uima/eclipse-update-site/.

## Installation

Clone the minimal pipeline from the repository with:

```
git clone https://github.com/mnicosia/minimalpipeline.git
```

Cd into the resources/ folder and execute the generate-types.sh script

Now go to the parent directory and type:

```
mvn compile
```

Then

```
mvn clean dependency:copy-dependencies package
```

## Running the pipeline

```
./run.sh
```

Look into the run.sh script and the arguments/trec-en-pipeline-arguments.txt file to understand what is happening.  

## Importing the project into Eclipse



## Running an experiment

### Compiling SVMLightTK

Go to the tools/SVM-Light-1.5-rer/ folder and type:

```
  make clean  
  make
```
