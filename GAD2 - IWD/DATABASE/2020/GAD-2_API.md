**Module Name** – GAD-2 IWD (Web) 

**Student Mentor** – Kushagra Yadav (21BCS121) 

# **API Documentation of GAD-2 IWD Module** 

 ## **Overview of the module:-**  

The IWD Module within Fusion plays a crucial role in overseeing the upkeep of campus property and ensuring its efficient maintenance. 

Its primary responsibility is to guarantee the smooth functioning of all on-site assets, promptly addressing any malfunctions that may arise.  

Additionally, the IWD Module actively oversees and manages the construction of new properties, demonstrating a comprehensive approach to both maintaining existing assets and facilitating the development of new ones on the campus. 

This dual focus reinforces its commitment to the overall well-being and advancement of the campus infrastructure. 

**Please mention all the API used in the module below** 

1. /page1\_1 - Already implemented 
   1. Parameters required – aes\_file, dASAName, nitNiqno, proth, emdDetails, preBidDate, technicalBidDate, financialBidDate. 
   1. Description - Stores all the important details related to the work being done with respect to the request approved. 
1. /page2\_1 - Already implemented 
   1. Parameters required – corrigendum, addendum, preBid, technicalBid, qualifiedAgencies, financialBid, lowAgency, letterOfIntent, workOrder, agreementLetter, milestones. 
   1. Description – Stores all the necessary information and documents required for the work which is issued. 
1. /corrigendumInput – Partially Implemented 
1. Parameters required – id, issueDate, nitNo, name, lastDate, lastTime, env1BidOpeningDate, env1BidOpeningTime, env2BidOpeningDate, env2BidOpeningTime. 
1. Description – Users have the ability to address any errors that may have 

   occurred during the submission of their documents. 

4. /addendumInput - Already implemented 
1. Parameters required – id, issueDate, nitNiqNo, name, openDate, openTime. 
1. Description – Users have the option to submit updated documents in case any errors persist in the previous versions. 
5. /milestoneForm - Already implemented 
   1. Parameters required – id, description, timeAllowed, amountWithheld. 
   1. Description – The involved agencies have a specified time frame to resolve all matters related to the payment amount. 
5. /TechnicalBidForm - Already implemented 
   1. Parameters required – id, requirements. 
   1. Description – The agencies involved in the biding process are required to list down all the details and requirements.
5. /extensionForm - Already implemented 
   1. Parameters required – id, hindrance, periodOfHindrance, periodOfExtension. 
   1. Description – The agencies involved in the project can request an extension of the deadlines, providing proper reasoning. 
5. /letterOfIntent - Already implemented 
   1. Parameters required – id, nitNiqNo, dateOfOpening, agency, name, tenderValue. 
   1. Description – The agency communicates its intent regarding the assigned work, providing all the necessary details. 
5. /workOrderForm - Already implemented 
   1. Parameters required – id, issueDate, nitNiqNo, agency, name, amount, time, monthDay, startDate, completionDate deposit, contractDay. 
   1. Description – The agency lists down the details for their assigned work. 
5. /agreement - Already implemented 
   1. Parameters required – id, date, dateOfOpening, agencyName, workName, fdrSum. 
   1. Description – The agencygives a formal agreement for their assigned work. 
5. /page3\_1 - Already implemented 
   1. Parameters required – id, extensionOfTime, ctualCostOfBidding. 
   1. Description – The agency is required to submit necessary details if they seek an extension. 
5. /page1View – Partially implemented 
   1. Parameters required – NIL. 
   1. Description – The administrator can check the details submitted in the page1\_1 form. 
5. /page2View - Already implemented 
1. Parameters required – NIL. 
1. Description – The administrator can check the details submitted in the page2\_1 form. 
14. /page3View - Already implemented 
    1. Parameters required – NIL. 
    1. Description – The administrator can check the details submitted in the page3\_1 form. 
14. /extensionFormView - Already implemented 
    1. Parameters required – NIL. 
    1. Description – The administrator can check the details submitted in the extension form. 
14. /financialBidView - Already implemented 
    1. Parameters required – NIL. 
    1. Description – The administrator can check the details submitted in the numberOfEntriesFinancialBid form. 
14. /numberOfEntriesTechnicalBid - Already implemented 
    1. Parameters required – number. 
    1. Description – The administrator has the capability to review bid details associated with the project ID "number". 
14. /numberOfEntriesFinancialBid - Already implemented 
    1. Parameters required – description. 
    1. Description – The agency has the option to submit details pertaining to their financial bids. 
14. /preBidForm - Already implemented 
    1. Parameters required – id, nameOfParticipants, issuesRaised, responseDecision. 
    1. Description – All the bid details are submitted using the provided form. 
14. /AESForm - Already implemented 
    1. Parameters required – id, descOfItems, unit, quantity, rate, amount. 
    1. Description – The agency is required to submit all the necessary items for their work, including their proposed price, quantity, and other essential details. 
14. /workOrderFormView - Already implemented 
    1. Parameters required – NIL. 
    1. Description – The administrator can check the details submitted in the workOrder form. 
14. /letterOfIntentFormView - Already implemented 
    1. Parameters required – NIL. 
    1. Description – The administrator can check the details submitted in the letterOfIntent form. 
14. /preBidDetailsFormView - Already implemented 
1. Parameters required – NIL. 
1. Description – The administrator can check the details submitted in the preBidDetails form. 
24. /technicalBidView - Already implemented 
    1. Parameters required – NIL. 
    1. Description – The administrator can check the details submitted in the technicalBid form. 
24. /milestoneView - Already implemented 
    1. Parameters required – NIL. 
    1. Description – The administrator can check the details submitted in the milestone form. 
24. /addendumView - Already implemented 
    1. Parameters required – NIL. 
    1. Description – The administrator can check the details submitted in the Addendum form. 
24. /corrigendumView - Already implemented 
    1. Parameters required – NIL. 
    1. Description – The administrator can check the details submitted in the Corrigendum form. 
24. /agreementView - Already implemented 
1. Parameters required – NIL. 
1. Description – The administrator can check the details submitted in the Agreement form. 

APIs:- 

- **Already Implemented (**This means that API is already implemented and working as expected.**)** 
- ![GAD-2 IWD Use Case Diagram](GAD-2_UCD.jpg)
- *issue\_work\_order -  UC#2* 
- Index of api’s used -  9 
- Description – The agency lists down all the details related to their assigned work. 
- Database - iwdModuleV2\_workorderform 
- **Yet to be implemented or Partially Working** (API is not implemented so yet to be implemented or API is partially working i.e it has breakage.)** 
- *Create\_new\_request - UC#1*** 
- Index of apis used - NIL 

- *Forward\_complaints–* UC#10 
- Description – The user will have the ability to initiate a new request for the construction or maintenance of any property. 
- Database - No table created 
- *Process\_request - UC#5*** 
- Index of apis used - NIL 
- Description – The dean processes the request created by the user. 
- Database - No table created 
- *audit \_final\_bill* - UC#4** 
  - Index of apis used - NIL 
  - Description – The dean audits the final bill generated by the agency and settled by the account admin. 
  - Database - no table created 
- *Approve/reject\_request* - UC#6 
  - Index of apis used - NIL 
  - Description – The director will approve or will ask to reform the request processed by the dean. 
  - Database - no table created 
- *Audit\_document –* UC#7 
  - Index of apis used - NIL 
  - Description – The auditor audits all the documents submitted by the users and can ask them to re-submit them in case of any errors. 
  - Database - no table created 
- *Settle\_bill–* UC#8 
  - Index of apis used - NIL 
  - Description – The account admin processes the settlement of the bill after it is generated by the agency. 
  - Database - no table created 
- *Manage\_inventory –* UC#9 
- Index of apis used - NIL 
- Description – The IWD admin oversees the management of all available resources and initiates requests for the availability of resources that are currently lacking to ensure the efficient operation of the team. 
- Database - no table created 
- Index of apis used - NIL 
- Description – The complaint manager forwards all listed complaints to higher authorities for further review and resolution. 
- Database - no table created 

**Current problems you are facing with the module or in its use cases —** 

- The use case diagram has been recently updated, resulting in a situation where the majority of the specified use cases are yet to be implemented. 

Google Doc Link :[ Modules Testing Assignment.docx](https://docs.google.com/document/d/1YHGPKiRUQ0TMEIk8w4HZ7sWOhSeqEkCdI3leq7ubZ_k/edit?usp=sharing)

\--------------------------------------------------------------------------------- 
