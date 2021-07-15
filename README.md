# Spark Plugin Example
This is an example to illustrate how to build a plugin for Spark. You can use this repo as a template and add/change Spark code. 

## how to build 
Build with `mvn clean packge` command, and it will generate a jar in `target` folder

## how to use
Add such configs in your `spark-defaults.conf` file
```
spark.files                         file:///absolute/path/to/your/jar/file
spark.executor.extraClassPath       ./your-jar-file-name
spark.driver.extraClassPath         file:///absolute/path/to/your/jar/file
```