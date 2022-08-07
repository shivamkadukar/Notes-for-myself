1. Install java 8 or later.

      [openlogic java jdk](https://www.openlogic.com/openjdk-downloads)

2. Setup JAVA_HOME environment variable

   `JAVA_HOME = C:\Program Files\OpenJDK\jdk-8.0.262.10-`
   
3. Add JAVA_HOME to path

    `C:\Program Files\OpenJDK\jdk-8.0.262.10-hotspot\bin`

4. Install spark with hadoop.

    [spark download](https://spark.apache.org/downloads.html)

5. Unzip the tar file and save it a specific folder of choice.

6. Windows has some more dependencies which need to be installed.
    * winutils.exe required to run spark on windows,  
    * hadoop.dll required to convert spark dataframe to parquet.  
Install these files and save it in bin folder of spark hadoop.

    [windows utils for spark-hadoop](https://github.com/cdarlint/winutils)

7. Environment variable to be setup 

    `PYSPARK_PYTHON = C:\Users\dell\AppData\Local\Programs\Python\Python38\python.exe 
    PYSPARK_DRIVER_PYTHON = C:\Users\dell\AppData\Local\Programs\Python\Python38\python.exe 
    SPARK_HOME = C:\Apps\spark-3.2.1-bin-hadoop3.2 
    HADOOP_HOME = C:\Apps\spark-3.2.1-bin-hadoop3.2`

8. Add the location of spark bin folder to path

    `C:\Apps\spark-3.2.1-bin-hadoop3.2\bin`


