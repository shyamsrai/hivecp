# hivecp

A simple script to consolidate the steps of copying/transferring Hive specific data between two Hadoop clusters. The approach is based on the following steps.

1. Source hadoop cluster has hive database with couple tables and metadata stored in Mysql database
2. Data is transferred using distcp (as oppposed to export/import), on target cluster since it requires some overhead steps
3. Metadata is restored on the target cluster
4. Everything is supposed to work fine

