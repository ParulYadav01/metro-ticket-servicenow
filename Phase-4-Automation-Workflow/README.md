Data Handling:
Store ticket data in the Metro Database  table with references to user entries.

Variables to Custom Table Records

·      In this Case I used Process Automation technique to Capture the Variables through the catalog item and are automatically mapped and stored in a custom table (Metro_Database) for structured tracking.

Process to map the variables as shown below.

·        Create a flow in flow designer and add Trigger points as per our requirement.

·    Select/Use Get Catalog Variables Action to access the Variables from Service Catalog.

·        User Create/Update record action and Select the Metro database.

·  Click on Add fields (+) icon to Map the Variables to particular fields as per our requirements.

Access Control:
Created Role-Based ACL’s

Users/Clients are directly able to Book  a ticket or recharge Metro card, But they can not access the Database table.

While creating a custom table 4 ACL’s are created automatically, in this scenario I used the default ACL’s only

QA Testing:
Catalog testing for form behavior, QR Generation and visibility.

Data Integrity:
Field validations: non-empty source/destination, fare match, approved travel date.

       Field Validation and Automation

·  Mandatory Fields: Enforced on client and server side to prevent incomplete submissions.

·     Auto-Populate Logic: Set up default values (e.g., single, return journey) using catalog client scripts and UI policies.

·     Fields Mapping : used Process Automation Engine to Auto mapping the fields  and populate the values which are given by the user/clients.
