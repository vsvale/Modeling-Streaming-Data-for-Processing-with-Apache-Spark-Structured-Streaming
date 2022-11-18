# [Modeling Streaming Data for Processing with Apache Spark Structured Streaming](https://app.pluralsight.com/library/courses/modeling-streaming-data-processing-apache-spark-structured-streaming/table-of-contents)

Streaming analytics can be difficult to implement. This course will teach you to model real-time data processing with Spark Structured Streaming.

### Description
Streaming analytics can be a difficult to set up, especially when working with late data arrivals and other variables. In this course, Modeling Streaming Data for Processing with Apache Spark Structured Streaming, you’ll learn to model your data for real-time analysis. First, you’ll explore applying batch processing to streaming data. Next, you’ll discover aggregating and outputting data. Finally, you’ll learn how to late arrivals and job failures. When you’re finished with this course, you’ll have the skills and knowledge of Spark Structured Streaming needed to combine your batch and streaming analytics jobs.

### Author
[Eugene Meidinger](https://app.pluralsight.com/profile/author/eugene-meidinger)

### Platform
[Pluralsight](pluralsight.com/)

### Notes

#### Install Pyspark
- `pip install pyspark`
- if jav anot installed: 
  - `sudo apt install default-jre`
  - `export JAVA_HOME=$(dirname $(dirname $(readlink -f $(which java))))`
  
#### Blood samples
- Run server to generate blood samples: `python3 server1.py`
- Run select.py to get these blood samples, filter negative bloodGlucose ones and print to console: `python3 selecet.py`

#### Group and Agg
- samples increasing and decreasing values: `python3 server2.py`
- Run avarage.py to group increasing and decreasing values by it kind and by event time, every 30s is a new group: `python3 avarage.py`

#### Watermark
- samples: `python3 server3`
- through away everithing older than 1 hour: `python3 watermark.py`
