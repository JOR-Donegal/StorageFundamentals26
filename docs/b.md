# Storing Data

There are some different terms we use for how data is aggregated and stored. Sometimes we deal with data one character at a time. In Unix for example, devices can be _character based_, like a keyboard or a mouse. 

## Block Storage ##
For efficiency and for structure data, we store data on disks in blocks of a fixed size and we call this _block storage_. A block is a sequence of bits or bytes of a fixed length, determined by the underlying system. Imagine a 64-bit system; things get really confusing once we store multiple bytes, we could store the most significant byte first or last. We have terms like big-endian and little-endian to describe this. Secondary storage is block storage, with disks being broken up into sectors, originally of 512 Bytes, these days of 4,096 Bytes. For efficiency, some file systems aggregate these sectors further into blocks or clusters. 

In data centre work, we abstract and aggregate disks into a single device for block storage, using a network to share volumes of data amongst many servers. Adding a disk array to a volume manager gives us a device called a _Storage Area Network_ (SAN). 

Originally, we stored data directly on disks and for reliability, we used reliability techniques like the _Redundant Array of Independent Disks_ (RAID), which will be explained in later lectures. 

## File Storage
One of the earliest applications on a LAN was for file sharing from _file storage_.

A _file server_ was a generic case of _Direct Attached Storage_ or DAS. 

Unstructured data may be stored as file data although hidden underneath the file store, we probably have block storage. For file-based storage we use a _Network Attached Storage_ system or NAS; imagine this as a SAN with a file system manager as a front end. 

## Object Storage
And there is yet another category which has emerged primarily for unstructured data, _Object Storage_. Each object contains data, meta-data, and a _Globally Unique Identifier_ (GUID). If you are saving photos or audio to the cloud, this is probably the format the data is in. In Amazon S3 buckets, everything is an object. However, it will sit on a backing store that is almost certainly block-based. Object storage is an abstraction of the underlaying technology. 

## Streaming
Just when I had my categories and headings just right, along comes a completely different way of looking at data.

Streaming data refers to a continuous flow of real-time data that is generated, processed, and transmitted in a steady and uninterrupted manner. This data is typically produced by various sources, such as cameras, sensors, devices, applications, social media, and other sources that continuously generate information.

A _streaming data platform_ (SDP) is a system that processes that data as it streams, rather than at rest. It operates and processes the data in real-time, continuously. Read a little bit about [Apache Kafka](https://kafka.apache.org/) to understand a typical platform.

In 2024, I worked on an SDP project on a platform from Dell, just before they discontinued the product!


