# B2SHARE Training Module
<img align="right" src="img/B2SHARE-logo.png" alt="B2SHARE logo" text="B2SHARE logo"> This training module provides training material and in-depth information in using the [EUDAT B2SHARE service](https://trng-b2share.eudat.eu) using programmatic interfaces. It covers API usage and implementation and provides step-by-step implementation examples using Python.

All submodules have been set up to use the [B2SHARE training instance](https://trng-b2share.eudat.eu), which you can freely try and experiment with.

Please note that in order to use the services you need to register your account and log in. Click [here](https://trng-b2share.eudat.eu/youraccount) to do so.

This module is work in progress and subject to change. Since B2SHARE is currently in development, the API might change as well. As soon as there are updates, this training module will be updated as well. In the meantime, you can check out the currently up-to-date [API implementation](https://trng-b2share.eudat.eu/docs/b2share-rest-api) on the B2SHARE website.

### Prerequisites
This training modules assumes you have knowledge about data management basics such as depositing, metadata and persistent identifiers. In addition, all scripts are written in the [Python scripting](http://python.org) language. If you have no experience in programming or want to learn more about Python, it is highly recommended to follow [some](https://www.stavros.io/tutorials/python) [tuturials](http://pythonprogramminglanguage.com) or start [reading](https://en.wikibooks.org/wiki/Python_Programming) about it.


For trainees who do not have the possibility to install Python and the required Python packages, EUDAT provides pre-installed virtual machines in a training environment. To get access to this training environment, please use the [EUDAT contact pages](https://eudat.eu/support-request?service=DOCUMENTATION). Please provide some details on which community you are from and in which context you would like to follow the tutorial. 

### Important remarks
The B2SHARE service makes a distinction between the two terms `record` and `deposition`. A record is unchangeable and has a persistent identifier (PID) assigned to it. A user can create a record by first creating a deposition, which is modifiable until finally committed. Files and metadata can be placed into a deposition, but not into a record. 

In practice, a record is equivalent to a deposition when solely trying to read a record through the service API. When creating new records, this has to be done using a deposition since it is created before any metadata or files are added.

There is no difference between a `record` and a `deposit`, these terms can be used interchangeably.

### Submodules

Submodule | Contents
------|-------------
[Getting your API token](00_Getting_your_API_token.md) | Information on registration and creating your API tokens for usage with the Python scripts
[Retrieve record details](01_Retrieve_existing_record.md) | Learn how to get deposit information of specific existing records
[List existing records](02_List_existing_records.md) | Retrieve listings of records and paginate them
[Create new deposit](05_Create_new_deposit.md) | Learn how to create new deposits and add files and metadata
[Example script](10_Example_script.md) | Example script with functions handling B2SHARE deposits
[Appendix A](A_Setup_and_install.md) | Setup and install guide for Python
[Appendix B](B_Request_and_Metadata_Reference_Guide.md) | Reference guide for API requests and record metadata
