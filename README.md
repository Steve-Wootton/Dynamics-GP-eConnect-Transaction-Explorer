The eConnect Transaction Explorer is a graphical front end application for Microsoft Dynamics GP eConnect.
* Refer to the Wiki pages (link above) for information regarding installation and use.
* Click the Releases link (link to the right) to get a list of releases.

## Overview
Microsoft Dynamics Great Plains, or simply *GP*, has an API that is referred to as *eConnect*. eConnect is based on XML-formatted messages and is primarily used to move data into GP. It provides similar functionality to what is available through the standard GP user interface, with some exceptions.

The eConnect Transaction Explorer is an application that allows the user to easily explore all of the available eConnect transactions, select transactions to execute and populate transaction data, and to test/execute transactions against GP, all in a convenient graphical interface. For example, here is a screenshot of a sample GL transaction with two distributions that has been tested successfully against a running instance of GP:

![Sample GL Transaction](https://github.com/Steve-Wootton/eConnect-Transaction-Explorer/blob/main/screenshots/Sample_GL_Transaction.png?raw=true "Sample GL Transaction")

## Features
* Explore eConnect transactions.
* Select any eConnect transaction to test or execute.
* Within an eConnect transaction, select any combination of eConnect nodes (taXXX).
* Within the selected eConnect nodes, select any combination of elements (fields).
* Populate the selected eConnect elements with data.
  * Use a pop-up calendar to populate date fields.
  * Use a combo box populate fields that are limited to a set of values, such as SOPTYPE.
  * Query for pre-existing data within GP, such as available Batch IDs, Currency IDs, etc.
  * Get the next available value for JRNENTRY, SOPNUMBE, etc. elements.
* View and copy the eConnect XML for a transaction.
* Test an eConnect transaction against GP without commiting any data.
* View multiple transaction errors instead of a single error. For example, if you have a GL transaction with multiple distributions and several of the distributions have invalid account numbers or account indexes, each invalid account will be reported instead of only the first.
* When satisfied with the entered data, you can execute the transaction and commit the data to GP.
* Save transactions to a file.
* Load transactions from a file, whether saved by the eConnect Transaction Editor or by other applications.
