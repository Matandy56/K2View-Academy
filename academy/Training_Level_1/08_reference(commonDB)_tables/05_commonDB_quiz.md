# Reference Tables & commonDB Quiz

## ![](/academy/Training_Level_1/03_fabric_basic_LU/images/Quiz.png)
Excellent! 
You have completed the commonDB items.


Take the following Quiz to see what you have learnt. 

The Quiz consists of of multiple-choice questions, each providing a number of possible answers. 

Click the answer you think is correct. 



#### Question 1: Reference Tables

Reference Tables are:

A: Tables keeping data in SQLlite format.

B: Oracle SQL tables used as data model references to create a new LU.

C: Statistics and maintenance tables, part of the LU schema tables .


(**Solution 1: A**).




#### Question 2: Creation of Reference Tables

New Reference Tables can be created from:

A: Within the LU schema.

B: Within the Reference folder in Fabric Studio (and only from there).

C: Cassandra CQLSH command line 

D: Fabric runtime console.

E: All of the above

(**Solution 2: B**).




#### Question 3: commonDB Type

commonDB is a supplementary Fabric database of the following type:

A: Cassandra.

B: mySQL.

C: SQLite

D: postGrSQL.

(**Solution 3: C**).



#### Question 4: commonDB Location

How many copies of commonDB can be found in a Fabric Cluster?

A: One only (it is common ...)

B: One for each Fabric node within the cluster.

C: Multiple - it is configurable depending on the need. 

D: One per Reference Table - a new copy of commonDB is kept for each Reference Table

(**Solution 4: B**)



#### Question 5: Reference Tables Synchronization

Reference tables can be synchronized from their external sources,

A: Once a day at a given time.

B: According to a specific schedule (CRON or functions).

C: Upon user request only

D: All of the above

(**Solution 5: D**)



#### Question 6: Reference Tables Cross-Nodes Updates

Reference tables are synchronized (between nodes) across the Fabric Cluster 

A: Each time a change occurs in the table using Queue Messaging topics.

B: Once day at a given time.

C: According to a specific schedule.

D: Upon user request only.

E: All of the above

(**Solution 6: A**)



#### Question 7: commonDB Runtime Status Commands

Reference Tables synchronization status for all tables can be displayed using the following command:

A: STATUS_REF ALL;

B: REF_STATUS TABLES=’ALL’;

C: REF_STATUS TABLES=’ALL’;

D: REF_SYNC_WAIT 'ALL';

(**Solution 7: B**)



#### Question 8: Reference Tables Synchronization Statuses

If a request for sync has been issued but not yet started, the status will be:

A: IN_BACKGROUND_SYNC

B: WAITING_FOR_SYNC

C: IN_SYNC
Sync in process.

(**Solution 8: B**)



#### Question 9: Session's Transaction values

A transaction that has been successfully reverted will show which one of the following status?

A: STARTED

B: COMMIT COMPLETED

C: ROLLED BACK

(**Solution 9: C**)



#### Question 10: Reference Tables Updates

What needs to be done to ensure that the most updated Reference Table data is available when accessing a specific LUI.

A: Attach the Reference Table to the LU schema

B: Run a SQL JOIN query from the Data Viewer

C: Run a Ref_sync command from the console

D: Nothing needs to be done as it happens automatically in the background

(**Solution 10: A**)



#### Question 11: Session's Transaction values

How can you query a Reference Table from an LU Population or Enrichment Function?

A: Attach the Reference Table in the LU (check in the Reference Table Tab)

B: Query a Reference Table from an LU even if it is not attached to the LU

C: It cannot be done from a population or enrichment function

(**Solution 11: B**)



#### Question 12: Reference Table Access from a Web Service

How do you make sure the most updated data of the reference table is available when invoking a Web Service?

A: Use both ref_sync and ref_sync_wait fabric commands from the web service java code

B: It cannot be done unless you refer directly to the LU from the Web Service after attaching the Reference Table

c: Web services always trigger automatically a background synchronization process for all Reference Tables defined in the project

(**Solution 12: A**)


[![Previous](/articles/images/Previous.png)](/academy/Training_Level_1/08_reference(commonDB)_tables/04_commonDB_solutions.md)

------
