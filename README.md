# Minimal Structural Reranking Pipeline

Thisi is a stripped down version of the reranking pipeline.  

With this software you will be able to apply structural reranking on a question answering dataset.

## Prerequisites

### UIMA

Go to https://uima.apache.org/downloads.cgi and download the latest binary distribution of UIMA.  

Decompress the archive and set the $UIMA_HOME environmental variable to the bin/ folder in the
UIMA distribution directory. You can use export="path/to/dir" if you use Linux/Mac and add this line
to ~/.bashrc in order to automatically set it in the future.

