# Ticket Response Codes

This is a table of INFOrm response codes and the rules describing their meaning and how they are used.
- For the instructions on ticket handling, please see WORKING TICKETS 
- For a step by step process, please see MY VERY FIRST TICKET 
- For ticket response codes, please see TICKET RESPONSE CODES 
- For ticket Incident Change Code usage see INCIDENT MANAGEMENT - CHANGE DEPLOYMENT REPORT ICT
- For a step by step process on creating a Child ticket, please see CHILD TICKET
- For an in-depth look at ticket closure, plsee see CLOSE TICKET
- For missed target (past SLA) tickets, please see MTRGT
- For unactionable tickets, please see VERIFIED/NO ACT TICKET PROCEDURE
- For accessing and uploading files attached to tickets, please see TICKETS: ATTACHED FILES


## Work Update Codes
Everyday response codes used for working tickets.

| INFROrm Code | INFOrm Label | Description|
| :-------------|:--------------|:------------|
|TECAT|WORK IS IN PROGRESS|Dispatchee assigns responsible technician. The TECAT Code can not be used for incidents on hold.|
|TECSU|WORK PROGRESS CONTINUES|Technician notes/comments. Can be used multiple times. The TECSU Code can not be used for incidents on hold.|
|TECRI|RESOLVED PENDING CONFIRMATION|Technician adds final notes/comments indicating resolution of the issue. The TECRI Code can not be used for incidents on hold.|
|TECNR|WMS TICKET NOT RESOLVED|TECNR is used to indicate the incident is not resolved after a TECRI. Removing the responsible technician from the ticket and adding the TECNR response code moves the ticket to the unassigned step to be worked. Leaving the responsible assigned technician on the ticket and adding the TECNR response code moves the ticket to assigned pending technician for the technician to work the ticket.|
|DSPOK|DISPATCHEE CONFIRMED CUST OK TO CLOSE|Response code used by the technician who contacted the customer to verify that the incident has been resolved. Requires a phone call or email to the customer by the technician, dispatchee or CIM technician. When entering, technician must also include the customer's name (first and last) for incident tickets, and for monitor tickets, an employee ID.|
|COMNT|1 TSC TECH COMMENTS|A generic comment.|	A generic comment.|
|TECAI|INFORMATION ADDED FOR CLARIFICATION|A more specific comment.|
|TECWC|INFORMATION REQUIRED FOR CUSTOMER|Indicates the technician is waiting on the customer for information regarding the incident.|
|TECIR|INFORMATION RECIEVED FROM CUSTOMER|Indicates the technician has received the requested customer information regarding the incident.|

## QA Codes
Response Codes that require interaction with TSC/CIM
1. Dispatch must contact the proposed dispatchee to discuss ownership change of incident.
2. Dispatch must contact CIM in order to request the change in ownership of the incident.

|INFOrm Code | INFOrm Label | Description|
|:-----------|:-------------|:-----------|
|TECWA|WMS TECHNICIAN WRONG ASSIGNMENT|Technician, wrong assignment. If the original dispatchee determines their area should not have received the request the dispatchee will document the incident with a response code of TECWA and contact CIM to transfer the incident. If the CIM technician agrees with the reassignment the TECWA response code will be added with the accompanying documentation on the call. When the transfer takes place the dispatchee will remove all steps from the original dispatcher's view and add an unassigned step to the new dispatchee view.|
|TECOC|WMS TECHNICIAN OWNERSHIP CHANGE|Used by the dispatchee to document a change in ownership because the resolution belongs entirely to another support area. Requires 2 phone calls:|
|TSCQC|TSC QUALITY CONTROL|Used for situations when First Level documentation in a ticket is incorrect or missing, or other situations when TSC process was not followed properly.|
|TSCFC|TSC FCR CANDIDATE|Used for situations when First Level Support should have had the ability to resolve the issue. Document the necessary steps to resolve the issue under this code and possibly get an ISKB created for the TSC to reference in the future.|

## Hold Codes
If waiting on a future event, placing the ticket on hold will halt the need to provide regular updates in the ticket until it is taken off of hold or the hold expires. Using the HDXX codes will immediately place the ticket on hold after a hold expiration date is provided, so be sure to update the ticket's ECD to match the hold date before entering your HDXX code.

|INFOrm Code | INFOrm Label | Description|
|:-----------|:-------------|:-----------|
|TECHD|	WMS TECHNICIAN REQUEST HOLD|	Application placed on hold after response code TECAT was added to the incident and the timer expired prior to the assigned technician adding an appropriate response code. Adding TECHD response code will reset the timer and move the incident to the next step.|
|TECHR|	WMS TECHNICIAN REQUEST HOLD REMOVAL|	Hold complete, early hold release. If a technician needs to request an early hold release the TECHR response code is used. The technician should provide appropriate documentation for informational purposes.|
|HDBC|	WAITING ON BATCH PROCESS TO COMPLETE|	Hold pending a batch cycle to run for customer to verify that the issue has been resolved.|
|HDCC|	WAITING ON ADDITIONAL CODE CHANGE|	Hold pending a software code change to resolve issue.|
|HDCI|	WAITING ON CUSTOMER INPUT|	Hold pending a customer response. Customer is absent and no backup exists.|
|HDEC|	WAITING ON EQUIPMENT FROM CUSTOMER|	Remote customer - waiting on equipment to be brought in by customer.|
|HDEX|	WAITING ON EXTERNAL VENDOR|	Waiting on external vendor to repair or correct issue.|
|HDFD|	WAITING ON FUTURE DATE TO BEGIN WORK|	Customer request made to hold work until a future date. Customer to request X days for hold or specific date.|
|HDFT|	WAITING ON EXTERNAL DATA|	Hold pending file transfer or external data delivered by customer.|
|HDPO|	PARTS ON ORDER|	On hold pending parts delivery or software from an external vendor.|
|HDPR|	WAITING ON PURCHASE REQUISITION|	Hold pending a purchase request and fulfillment initiated by the customer.|
|HDSD|	WAITING ON SOFTWARE DELIVERY|   Hold pending a software delivery required to correct issue. Software change/update may be required (SMS push).|

## Other Codes

|INFOrm Code | INFOrm Label | Description|
|:-----------|:-------------|:-----------|
|SUPH| SUPPORT HOURS| Used when Support Hours are approved for Development work on a ticket. When using this code, supply the following information:

1. The name of the Development Team Lead.
2. The number of hours approved.
3. The ETKS code to which the hours are charged.
4. The ECD of the development task.
5. A short description of the development task.
6. The name of the person who approved the support hours. |

## Resolution Codes
|Code | Description|
|:-----------|:---------|
|1CU|	CUSTOMER RESOLVED W/OUT I/S ASSISTANCE|
|1ED|	PROVIDED CUSTOMER EDUCATION|
|1RB|	REBOOT|
|1RE|	OTHER ACTION TAKEN RESOLVED THE ISSUE|
|1REIN|	REINSTALL/ UNINSTALL SOFTWARE|
|1RP|	RESET PASSWORD / UNLOCKED ACCOUNT|
|1RPRT|	RECYCLED PRINTER / SPOOLER|
|1RTOI|	RELATED TO PREVIOUS ISSUE|
|1SI|	SOFTWARE INSTALL|
|1UN|	UNABLE TO RECREATE THE PROBLEM|
|3APP|	APPLICATION ISSUE|
|AMBR|	AMBER LIGHT ISSUE RESOLVED|
|BCKUP|	RESTORE FILE FROM TAPE BACKUP|
|DRVSP|	SERVER DRIVE SPACE CORRECTED|
|DUPT|	DUPLICATE TICKET|
|NODWN|	NO DOWNTIME ENTERED|
|POWER|	POWER PROBLEM AT SITE HAS BEEN CORRECTED|
|REJ00|	REJECTED|
|RFCR|	RFC REQUIRED FOR REQUEST|
|RSSVC|	RESTARTED SERVICES|
|SRVRE|	SERVER RESOURCE ISSUE CORRECTED|
|TSMMF|	TSM BACKUP ISSUE CORRECTED|
|VIAEX|	RESOLVED WITH EXTERNAL VENDOR SUPPORT|
|WITH|	WITHDRAWN WS13 VIRUS /SPYWARE/SPAM|
|WS15|	USER ERROR|
|WS7|	PRINTER FIX|
|WS8|	PRINTER ADD|
|WS9|	NETWORK PROBLEM / SUPPORT|

## Corrective Action Codes
|INFOrm Code | Description|
|:-----------|:-------------|
|A-CONFIG|	APPLICATION CONFIGURATION CHANGE|
|A-PATCH|	APPLICATION PATCH CORRECTED|
|A-REBOOT|	SERVER REBOOTED DUE TO APPLICATION ISSUE|
|BACKUP|	BACKUP RUN|
|BATCHJOB|	BATCH JOB RUN TO CORRECT PROBLEM|
|LDE-MGT|	BLADE CHASSIS ACCESS ISSUE CORRECTED|
|CERTIFICAT|	CORRECTED EXPIRED/INVALID CERTIFICATE|
|CHILDTKT|	CREATED CHILD TICKET|
|CUSTNR-NCA|	CUSTOMER NO RESPONSE-NO CORR ACTION|
|DEFECT|	POST-IMPLEMENTATION ISSUE|
|DSVIEW|	CORRECTED DSVIEW ISSUE|
|FAILOVER|	FAILED OVER TO SECONDARY|
|ISP|	INTERNET SERVICE PROVIDER|
|LOGRSCH|	RESEARCHED LOGS|
|N-FW|	FIREWALL ISSUE CORRECTED|
|N-HW|	NETWORK HARDWARE CORRECTED|
|N-ROUTING|	NETWORK ROUTING CORRECTED|
|N-SWITCH|	NETWORK SWITCHING CORRECTED|
|NASRESTORE|	NAS FILE OR SERVER RESTORED|
|PWRST|	RESET PASSWORD|
|RCHTK|	RESEARCH TICKET|
|RESTORE|	DATA-FILE RESTORE OR CORRECTION|
|RESTPOWER|	POWER RESTORED TO EQUIPMENT OR SITE|
|S-CONFIG|	CONFIGURATION ON SERVER CHANGED|
|S-DRVSPACE|	CLEARED SERVER DRIVE SPACE|
|S-HW|	REPAIRED/REPLACED SERVER HARDWARE|
|S-PATCH|	SERVER PATCH CORRECTED|
|S-REBOOT|	SERVER REBOOTED DUE TO SERVER ISSUE|
|S-REBUILD|	SERVER REBUILT|
|S-SECURITY|	SERVER SECURITY CORRECTED|
|STOR-CORR|	STORAGE DEVICE CORRECTED|
|SVC-RESTAR|	SERVICE RESTART|
|T-HW|	REPAIRED/REPLACED TELECOM HARDWARE|
|VENDOR|	VENDOR ISSUE|
|VERIFIED|	NO CORRECTIVE ACTION WAS TAKEN|

## Root Cause Codes
|INFOrm Code | Description|
|:-----------|:-------------|
|ACCT-LCK|	ACCOUNT LOCKED|
|APP|	APPLICATION CAUSED ISSUE|
|APP-ERR|	ERROR WITHIN APPLICATION|
|BLADE|	BLADE SERVER ACCESS ISSUE|
|CERTEXPINV|	EXPIRED OR INVALID CERTIFICATE|
|CHG-OTH|	CAUSED BY A CHANGE OTHER THAN RFC|
|CHG-RFC|	SCHEDULED CHANGED CAUSED ISSUE|
|CHGERR|	CHANGE ERROR|
|CONERR|	CONNECTIVITY/NETWORK ERROR|
|CONV-DATA|	CONV OF DATA/DB CAUSED ABENDS|
|CUS-TR-ERR|	CUSTOMER TRAINING/ERROR|
|DATA|	BAD DATA|
|DOMI|	DOMAIN/CONNECTIVITY|
|DSVIEW-KVM|	UNABLE TO ACCESS SERVER IN DSVIEW|
|DUPTICKET|	DUPLICATE TICKET|
|HDWRMAL|	HARDWARE MALFUNCTION|
|HWHS|	HEADSET FAILURE|
|HWPS|	POWER SUPPLY FAILURE|
|HWRP|	REPLACE PHONE|
|ICTNH-APP|	ICTNH OWNED APPLICATION|
|ISP|	INTERNET SERVICE PROVIDER|
|MON-CONFIG|	MONITOR CONFIGURATION ISSUE|
|MONT|	INTERNAL MONITOR SOFTWARE/HARDWARE ISSUE|
|MONT-HWFRW|	HARDWARE/FIREWALL CHANGE AFFECTED MONIT|
|NASDELETE|	NAS DELETE|
|NBP|	NOT BEING PURSUED PER MANAGEMENT|
|NET-CONF|	NETWORK CONFIGURATION CAUSED ISSUE|
|NET-HW|	NETWORK HARDWARE CAUSED ISSUE|
|NET-MOD|	NETWORK CHANGE CAUSED ISSUE|
|NETWKCHG|	NETWORK CHANGE|
|NETWKCONF|	NETWORK CONFIGURATION|
|NETWKHW|	NETWORK HARDWARE|
|NWCT|	NTWK CONNECTIVITY-EQPT DISCON/RECONNECT|
|NWSWI|	NET/SWITCH ISSUE-SEE PARENT TIC NET SERV|
|PRINTER|	PRINTER|
|PROCER|	PROCESS ERROR|
|PWRFAILURE|	POWER FAILURE TO EQUIPMENT OR SITE|
|RAVHW|	REMOTE ACCESS VPN HW-NON-FUNCTIONING HW|
|RAVSW|	REMOTE ACCESS VPN SW-NON-FUNCTIONING SW|
|REFCHLDTKT|	REFER TO CHILD TICKET|
|REFDEFECT|	REFER TO DEFECT # IN TEXT|
|REFPARTKT|	REFER TO PARENT TICKET|
|REMED|	REMEDIATION EFFORTS CAUSED ISSUE|
|S-DRVFULL|	SERVER DRIVE SPACE FULL|
|SER-REQ-ER|	REQUEST SUBMITTED INCORRECTLY|
|SRV-HW|	SERVER HARDWARE ISSUE|
|SRV-OS|	SERVER OPERATING ISSUE|
|STORAGE|	STORAGE DEVICE MALFUNCTION|
|T-HW|	TELECOM HARDWARE|
|T-3R|	RESULT OF A 3R MOVE|
|TBD|	TO BE DETERMINED|
|TSMMF|	TSM MISSED/FAILED|
|UNCONERR|	UNCONFIRMED ERROR|
|VENDOR|	EXTERNAL ASSISTANCE NEEDED FROM VENDOR|
