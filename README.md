---
project_name: atk-training-Pq
short_description: This is a project to mimic Persistent Queue mechanism with Sqlite3 as backend
tags: []
category: tech
long_description: >
  Develop an API which implements Persistent Queue mechanism with Sqlite3 as backend
  Built with poetry
---
Fix The following:
Pipeline to make sure the jobs submitted by producer are successfully processed by consumer.
If the jobs get crashed before successfully processing by consumer then the jobs are added to the queue again and pass to consumer

# Purpose
Persistent Queue manages the files produced by various producer programs and supply the generated files to the various Consumer programs in a conflict free mechanism.


# Installation
How do we use install the code, library or whatever. What prereqs are needed

# How to use it
Producer: If a producer uses a Pq library then it uses put_file() to write the generated file to write it in the sqlite3 table along with the timestamp
Consumer: If a consumer uses a Pq library and requests for the queued file using get_file() so it fetches in FIFO approach.

