# spark-ly

## Steps to set up pip and virtual env
1. python3 -m pip install --user --upgrade pip
2. python3 -m pip --version
3. python3 -m pip install --user virtualenv
4. python3 -m venv pyspark-besho-dataminer

## Activate the virtual env:
source pyspark-besho-dataminer/bin/activate

Install Spark
1. brew install apache-spark
2. pip install pyspark
3. pip install findspark

## Alternative Spark Installation

1. Download Spark from http://spark.apache.org/downloads.html
2. put it in your venv's bin folder
3. tar -xzf spark-3.1.2-bin-hadoop3.2.tgz
4. mv spark-3.1.2-bin-hadoop3.2 spark-3.1.2
5. ln -s /pyspark-besho-dataminer/bin/spark-3.1.2 /pyspark-besho-dataminer/bin/spark

## Add Java to ~ /.bash_profile
```
export JAVA_HOME=$(/usr/libexec/java_home)
export SPARK_HOME=~/spark-2.3.0-bin-hadoop2.7
export PATH=$SPARK_HOME/bin:$PATH
export PYSPARK_PYTHON=python3
```

## Use Java 8, set it in your bash:
1. /usr/libexec/java_home -V
2. export JAVA_HOME=`/usr/libexec/java_home -v 1.8.0_282`
3. java -version 

## Add Java-8 to ~ /.zshrc 
1. vim ~/.zshrc 
2. Add the following lines to the file
 ```
  export JAVA_HOME=$(/usr/libexec/java_home -v 1.8.0_282)
 ```
5. source ~/.zshrc
6. echo $JAVA_HOME
7. java -version
