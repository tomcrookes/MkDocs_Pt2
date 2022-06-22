# My Very First Ticket

So, you're ready to work tickets, huh? No? Well then, this should introduce you to the wonderful world 
of tickets! Below you will find a step-by-step guide to assigning, working, and closing out your very 
first ticket. It can be used as a reference as well, if you don't quite have it down by the first try... 
But you will, won't you?

- For the instructions on ticket handling, please see WORKING TICKETS 
- For a step by step process, please see MY VERY FIRST TICKET 
- For ticket response codes, please see TICKET RESPONSE CODES 
- For ticket Incident Change Code usage see INCIDENT MANAGEMENT - CHANGE DEPLOYMENT REPORT ICT
- For a step by step process on creating a Child ticket, please see CHILD TICKET
- For an in-depth look at ticket closure, plsee see CLOSE TICKET
- For missed target (past SLA) tickets, please see MTRGT
- For unactionable tickets, please see VERIFIED/NO ACT TICKET PROCEDURE
- For accessing and uploading files attached to tickets, please see TICKETS: ATTACHED FILES


## Reflection 
Launch a reflection session from your desktop (This is the shortcut with the text "3270" on the actual icon 
image and it should, by default, be named "Session 1" OR "Session 2" OR "Session 3". It doesn't really 
matter which one you use right now.).

After launching, you should come to a black screen, complete with text of all sorts of pretty colors (It's 
blue and green by default.)! The green text should read "BC/BS Enter Request". From here, type "cics" and 
press `Enter`. Doing so should bring you to a second screen, requiring your RACF User ID and password. Press `Enter`.


## INFO Info
You will now be transferred to a black screen with minimal text at the bottom. From here, type "info" and press `Enter`. 
This will bring you to the main menu of INFO.

By default, your cursor will automatically be placed in the "Enter Option" field. Enter the number for the option you 
would like to access (The arrow points to options 1, 2, 3, 5, 8, 9, A by default. Refer to the descriptions to the right 
of each for desired value). In this case, you will select option "9". This will take you to a summary view of your team 
members' ticket buckets. Next, your cursor will automatically start at the "UNASSIGNED" bucket line. Press `Enter` to select 
the line, and view its contents. If there are any unassigned tickets, this is where they will be stored. Most of the time, 
a ticket will already be assigned to you, but in this case yours is not.

Navigate the various tickets (if applicable), and press `Enter` to select a ticket (It is likely that your first ticket 
will be an S3 monitor ticket.). Pressing `Enter` brings you to the main ticket face, populated with the date of the incident, the description of the incident, contact information from the individual(s) experiencing issues, and much more. You can read through the brief description, and even press `F13 (SHIFT+F1)` to access the detailed view of the ticket. Here you will find more information about the incident.


## Let Me Show You How To Work It
Press `F3` to traverse backwards to the previous screen. Most likely, your first ticket will already be assigned to you (This means that the ticket will already be tagged with TECAT and TECSU response codes). If you are looking at the ticket face, you should see your employee i.d. next to the text `RSP TECH` in the lower right region of the INFO screen. To begin working on the ticket (from the ticket face), press `F14(Shift + F2)`. In the `RESPONSE CODE` field, input "tecsu". Tab down below the `~*~RESPONSE~*~` field, and input something simliar to "Currently researching the issue". Press ENTER. This will save your work, and you can press `F3` to go back to the ticket face. You will continue to update ticket with the **TECSU code**, leaving a comment relevant to your progess at the necessary intervals defined by the ticket severity's SLA.


## SLAy the SLA
Once you have come across a resolution to the issue, you will want to stop the SLA timer on the ticket, as not to leave a ticket live for longer than it needs to be. This mean you will need to, again, press `F14(SHIFT +F2)`, but this time you will enter **TECRI** in the response code section. Next, tab below the response section, and compose the following in the following format.

|   Problems    |       CAUSE       |       RESOLUTION  |
|---------------|-------------------|--------------------|
| This can be the user's stated problem just copied and pasted from the ticket detail view. | The problem was caused by this. | What you did to fix the problem...if nothing needed to be done, and the issue was resolved via monitor closeout, put NTI(stands for-->No Tech Intervention). |


## Stupid Screen!
After this is all done, press `Enter` to save and `F3` to go back to the ticket face. From here, you should press `F22(SHIFT + F10)` to access what is commonly referred to as the "idiot screen". Here you will find that you need to log similar information to what you just typed in the previous entry. the format will look a little something like this:

![InfoF22Screen](../img/InfoF22Screen.PNG)

Here, you will re-enter the problem in the **ACTUAL PROBLEM** area, and refer to the face of the ticket to find the **ACTUAL AREA** value (its located in the AREA field in the lower let corner of the ticket face..you can actually press `F1` to get a list of all of the areas) and input that. Next, **ASSET** will define the type of issue you are having (press `F1` while tabbed to the entry field to view options). You can leave **ASSET NAME** blank. Moving on, the value for **CORRECTIVE ACTION** most of the time, is **VERIFIED**. Check with a fellow teammate if unsure. Under **CORRECTIVE ACTION DESCRIPTION**, enter in more detail the corrective action you took to resolve the issue. For an S3 monitor ticket, it is often **NTI** (No Tech Intervention) and **Monitor has cleared**, to state that no actual action had to be taken to correct the issue.

For the final values--**ROOT CAUSE** and **ROOT CAUSE DESCRIPTION**, press `F1` to select the appropriate option and enter a description of what cause the issue below. Press `Enter`, and you are now done with te idiot screen! Press `F3` to go back to the ticket face.


## Hello, Mr. DSPOK!
**DSPOK** is the next code you will instantiate, stating that the problem has been resolved. And NO, it has no relation to Mr. Spock from Star Trek.

AS OF ***OCTOBER 2015***: In an effort to meet the expectations of the ISSM, and improve the quality of information in our tickets, the following standards for DSPOK-ing tickets has been mandated across all 'S' severity tickets.
- Incident Tickets - Customer name (both First & Last required) + corresponding verbiage "verified okay to close". For example: *John Doe verified okay to close*.
- Monitor Tickets - List the employee ID + corresponding verbiage "okay to close". For example: *MU18 okay to close*.

In order to enter the DSPOK code, from the ticket face hit shift + F2 and enter "DSPOK" in the RESPONSE CODE field. Tab down to the RESPONSE CODE DESCRIPTION: ***RESPONSE*** section and follow the criteria above to meet the expectations required to fill in the appropriate verbiage. Hit ENTER to lock in the information.

Finally, once the required steps have all taken place, hit `F2` to update the ticket face. Tab over to the **ACTION** field (upper right) and replace the asterisk with a "u". Tab down to **STAT field** (lower left) and replace "op" (open) with "cl" (closed). One last thing--tab over to **RESL** field and input the desired text ("notch" for no tech intervention--if something else, you can search through the list of codes by pressing F1 while the cursor is placed within the field). Once you do that, hit `Enter`. You ticket now disappears--it's closed. You just closed your first ticket! **Congratulations!**
