# Entity Matching POC

## Description
This project was inspired by issues I've encountered from time to time in my working experience. Having datasets where users manually enter business information leads to many differences and errors. It is difficult to identify which records belong to which company. These difficulties can be compounded when the companies on the list are volatile, often shut down, or have many satellite organizations with which they work. The overall goal of this project was to develop a process that minimizes manual work.  Also note that AI code generation was used for part of this process, as I was also experimenting with it at the same time.

### The process is broken down into several steps:  
* Data Cleaning and standardization  
* Split data for Test and Train  
* Use HDBSCAN to Cluster  
* Evaluate the result and isolate the "Good" Records  
* Review the "Good" Records. Lock them down  
* Match "Good" Records to using TDIF to exiting records  
* Then Repeat  

This process wasn't fully implemented; it was a POC to see if it was possible. The data_scramble.py file takes generated data and tries to mimic human mistakes for testing.

## Outcome  
Overall, I believe this can work with some more refinement.  

