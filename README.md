# Sparkling-Water-with-Python

Sparkling Water allows users to combine the fast, scalable machine learning algorithms of H2O with the capabilities of Spark. Spark is an elegant and powerful general-purpose, open-source, in-memory platform with tremendous momentum. H2O is an in-memory platform for machine learning that is reshaping how people apply math and predictive analytics to their business problems. Integrating these two open-source environments provides a seamless experience for users who want to make a query using Spark SQL, feed the results into H2O to build a model and make predictions, and then use the results again in Spark. For any given problem, better interoperability between tools provides a better experience.


=========== PySparkling

This section provides an introduction to PySparkling. To understand more about PySparkling, it’s best to first understand H2O, Spark, and Sparkling Water.

What is H2O?

H2O is an open-source, in-memory, distributed, fast and scalable machine learning and predictive analytics platform that provides capability to build machine learning models on big data and allow easy productionalization of them in an enterprise environment.

What is Spark?

Spark is an open-source, in-memory, distributed cluster computing framework that provides a comprehensive capability of building efficient big data pipelines.

What is Sparkling Water?
   
Sparkling Water is an integration of H2O into the Spark ecosystem. It facilitates the use of H2O algorithms in Spark workflows. It is designed as a regular Spark application and provides a way to start H2O services on each node of a Spark cluster and access data stored in data structures of Spark and H2O.
   
What is PySparkling?   
   
PySparkling is an integration of Python with Sparkling Water. It allows user to start H2O services on a Spark cluster from Python API.    


=== Used:   
Python- 3.5     
Anaconda- 4.2.0  
Spark- spark-2.2.0-bin-hadoop2.6     
pysparkling- h2o_pysparkling_2.2  
pyspark- 2.2.0 (already included in h2o_pysparkling_2.2  
   
== dependencies:   
colorama- 0.3.9  
requests- 2.19.1   
tabulate- 0.8.2  
future- 0.16.0  
six - 1.11.0  
    
------ Setting up PySparkling  
conda install -c gekas h2o_pysparkling_2.2        
link: https://anaconda.org/GeKas/h2o_pysparkling_2.2     
  
------ required dependencies:   
conda install -c anaconda colorama  
conda install -c anaconda requests  
conda install -c conda-forge tabulate   
conda install -c anaconda future  
conda install -c anaconda six  

========= Run PySparkling interactive shell  
  
1.  Ensure you are in the Sparkling Water project directory and run PySparkling  
  bin/pysparkling  
  
The pysparkling shell accepts common pyspark arguments.  
  
For running on YARN and other supported platforms please see Running Sparkling Water on supported platforms.  
  
2.  Initialize H2OContext  
  
  from pysparkling import *  
  import h2o  
  hc = H2OContext.getOrCreate(spark)  
   
  Run IPython Notebook with PySparkling:  
  $SPARKLING_WATER_HOME/bin/pysparkling    
  PARK_DRIVER_PYTHON="ipython" PYSPARK_DRIVER_PYTHON_OPTS="notebook"  
  or  
  PYSPARK_DRIVER_PYTHON="ipython" PYSPARK_DRIVER_PYTHON_OPTS="notebook" $SPARKLING_WATER_HOME/bin/pysparkling    
  



Reference:   
http://docs.h2o.ai/sparkling-water/2.2/latest-stable/doc/pysparkling.html    
 


