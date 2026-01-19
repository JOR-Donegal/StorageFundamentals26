# Classifying Data

We need to be able to distinguish between _data_ and _information_. 

As a technologist, I get to do lots of field science with other people, mostly during the summer months. In a week, we can gather a vast amount of raw data, for example on a bathymetric or a LIDAR survey, I will gather multiple MB/hour of raw position and depth data, with supporting fields indicating accuracy etc. If I’m doing side-scan, I can gather multiple GB/hour and for Photogrammetry, TB/hour. There is an old joke with field work that a week in the field takes a year to post-process and there may be truth to that. We clean and collate that data, add tidal compensation and then produce a three-dimensional graphic for a GIS system. The data in its raw form is unstructured, it cannot be meaningfully consumed or used. Processed and interpreted as a final report, it becomes information.

## Structured Data
How we treat and store data can depend on its type and an entire field of data science exists which we will not delve into! 

Where we have many records of data (rows) in fixed fields (columns), we construct two-dimensional tables and link these sets of data using keys which relate one piece of data to another. Such a database will have a well-defined data model or _schema_. A structure like this is a _relational database_ and a system to manage it is a _relational database management system_ (RDBMS). It can be very easy to query this kind of data and _Structured Query Language_ (SQL) is a standardized language for doing so for example

```
“FROM People SELECT * WHERE SurName = ORaw”. 
```

I began writing database programmes in early packages like dBase in the late 1980s. Compared to other programming languages, it was very easy to write data-centric applications. If you are not familiar with databases, their structure will make no sense. Do some background reading on |_database normalization_. For completeness, do some reading on NOSQL databases as well. 

## Semi-structured
Sometimes we deal with data which has a pattern and structure but is not defined by a fixed data model. Examples are spreadsheets or XML files. In data centre work, we commonly deal with JSON and YAML in addition to XML. 

## Quasi-structured data
In some cases, we store text data which can be further processed with time, effort, and good software! For example, the web logs of a system will show the sequence of pages accessed and the hyperlinks actuated to do so; this is a clickstream. 

## Unstructured data
Unstructured data does not fit in rows and columns, it may have little, or no classification or _meta-data_ associated with it; meta-data is data about data. Every time you take a photograph with an smart phone, it embeds location coordinates, time, and date, etc. in the file. This is an example of meta-data. An interesting thought…all of this would be personal data under GDPR, how many people have analysed the data they saved and considered the implications of the metadata. Much of our data is stored as files which have no inter-relationships or structure; a challenge for data management in a GDPR era. In most heterogenous environments, we see more growth in unstructured data than in any of the other categories. Some companies (who have a vested interest!!) claim unstructured data accounts for >80% of all stored data.

