# this is a stubb of a to be build "Glossary of Terms" for ERPNext

The intention is to build a Glossary of terms (i.e. 'Site', 'Form', etc.) and what they exactly mean in the logic of ERPNext
Initial goal is to help me understanding ERPNext and I will populate it as I go along discovering. Hopefully at some point others might add Definitions or correct/clarify this existing Glossary, and this might turn out to be useful for others as well

It is to be decided at what point it will be serious, big, good enough to do a PR to the orgiginal erpnext repository

===================================================

**Glossary of Terms**

**Site** - is something like the 'frame' for and ERPNext/frappe installation. It contains the database, backups, Apps. If one wanted to run multiple instances of ERPNext he/she would setup several 'sites'

**Like** (in Filter to filter list items) - same meaning as "Contains" (i.e Filter term 'SIN' will find Sales Invoices (SINV). "Like" has no ability to find misstyped terms though. It will not find 'tasks', when searching for 'taks'. 'Like' is not case sensitive

**Equals** (in Filter to filter list items) - will Filter the exact term which is put in. (i.e. Filter term 'SINV-0001' will find one specific Sales Invoice (SINV-0001). Neither 'SINV' nor 'SIN*' will find any Sales Invoice (SINV-xxxxx). 'Equals' is not case sensitive

**Filter** - [add definition here]

**Rate** (as in Sales Order, Invoices, ...) - the price per Unit sold/purchased

**Frappe Framework** - the Web Application ERPNext is build upon. It is delpoyable on any *nix Operating System (Linux, Unix, BSD, MacOS) [needs more knowledgeble explanation maybe]


**framework** - [add definition here]

**App** - a user programm which provides functionality (i.e. Accounting, CRM,...). An 'App' in this context has an API so it can connect to other apps

**API** - [add definition here]

**bench** - [add definition here]

**Frappe Technologies Pvt. Ltd.** - is the Company that has originally developed ERPNext and the frappe framework. I assume it is also the copyright owner of both.

**ERPNext Software Foundation** - is a yet to be started Foundation that, in order to guarantuee the Open Source Nature not being changed, shall overtake governance of the ERPNext and frappe Software. [question: will it become the copyright owner as well?] [needs more specification definetly]

**Submit** - by submitting a Document (Sales Order, Invoices, Jounal Vouchers [probably also Warehouse operations which I have not dealt with yet], etc.) it changes from being a draft (which actually does not yet have any impact on any values (like sum of money in a bank account, or Stock level of an Item) to an actual entry to the system which actual records something. 
Once a Document has been submitted it still can be withdrawn (Cancel) and adjusted (Amend) but these changes or cancellations are being recorded by ERPNext. If you 'Cancel' a submitted Sales Invoice (SINV-0001), 'Amend' it and re-submit this Amended version it will appear as SINV-0001-1 in your records. In order to be able to retrace such a change or cancellation the original document (SINV-0001 in our example here) will still be existing in a 'cancelled' state. It's value do not add up to the actual numbers though.

**Cancel** - you can 'cancel' a submitted document which means that it's impact on your system is being 'withdrawn'. If you cancel a 'Journal Voucher' for example the Voucher will still exist as a Document, but there will be now accounting entries in your accounts.

**Amend** - to change or adjust a cancelled document, so a correct Version of it can be submitted again. The original Document will continue to exist for traceablility reason. The Amended version will be named like JV-00001-1 (assuming the orignal (cancelled) Document was named JV-00001)

**Journal Voucher** - [add definition here]

**Sales Invoice** - [add definition here]

**Purchase Invoice** - has the same logic/functionality as a 'Sales Invoice'. the differnce being it is issued for Purchase from your Suppliers, so you have to pay money in order to receive goods (Items)

**Refresh** - [add definition here. should also explain difference to 'Reload']

**Reload** - [add definition here. should also explain difference to 'Refresh']



