# List of tables #

  * **lms\_jobs**: tracks all LMS-jobs (incl status and result)
  * **lms\_item\_list**: item updates are queued in this table
  * **accounts**: ebay accounts used by the seller

## Table: lms\_jobs ##

| **Field Name** | **Description** | **Field Type** | **Comment** |
|:---------------|:----------------|:---------------|:------------|
|uuid            |Unique ID of the LMS job|varchar(20)     |             |
|lms\_job\_id    |                 | | |
|file\_reference |                 | | |
|file\_reference\_result|                 | | |
|max\_filesize   |                 | | |
|timestamp\_start|                 | | |
|timestamp\_end  |                 | | |
|progress        |                 | | |
|status\_local   |                 | | |
|status\_ebay    |                 | | |
|result          |                 | | |
|message         |                 | | |

## Table: lms\_item\_list ##
| **Field Name** | **Description** | **Field Type** | **Comment** |
|:---------------|:----------------|:---------------|:------------|
|id              |INTEGER PRIMARY KEY AUTOINCREMENT| |                |
|lms\_uuid       |                 | | |
|seller\_item\_id|                 | | |
|xml             |                 | | |
|lms\_status     |                 | | |
|lms\_result     |                 | | |
|errors          |                 | | |
|errors\_msg     |                 | | |
|warnings        |                 | | |
|warnings\_msg   |                 | | |
|ebay\_item\_id  |                 | | |
|site            |                 | | |
|                | | | |

## Table: lms\_accounts ##
| **Field Name** | **Description** | **Field Type** | **Comment** |
|:---------------|:----------------|:---------------|:------------|
|id              |INTEGER PRIMARY KEY AUTOINCREMENT| |                |
|account\_id     |                 | | |
|token\_sandbox  |                 | | |
|token\_production|                 | | |
|primary\_site   |                 | | |
|                | | | |