DSC is an organization that helps non-profit organizations to find donors for their good causes. 
They have a huge database with candidate donors. DSC now wants to launch a new re-activation 
campaign where they want to send letters to donors that have been inactive for a long time, 
hoping that they will donate again. The CEO & Head of Data Analytics (conveniently, this is the 
same person for this exercise) have to be convinced that your model is better than just randomly 
selecting donors.
DSC is mostly interested in customers that have donated €30 or more, but you can be flexible in 
this decision, depending on your business case.

Datasets

DSC provides 5 datasets:
• donors.csv contains general information about the candidate donor database.
− donorID: The unique ID of the candidate donor.
− zipcode: The postal code of the candidate donor’s main address.
− province: The province of the candidate donor’s main address.
− region: The region of the candidate donor’s main address.
− gender: The gender of the candidate donor (M = male, F = female).
− language: The candidate donor’s preferred communication language (FR = French, NL 
= Dutch, EN = English).
− dateOfBirth: The date of birth of the candidate donor.
• gifts.csv contains information about the gifts that these candidate donors donated in the 
past for campaigns that are no re-activation campaigns
− donorID: The unique ID of the candidate donor.
− campaignID: The unique ID of the campaign (donation was made outside of a campaign 
if missing).
− amount: The amount of the donation (in EUR)
− date: The date of the donation payment.
• selection campaign 6169.csv: donors that were selected for a previous re-activation 
campaign on 04/09/2018.
• selection campaign 7244.csv: donors that were selected for a previous re-activation 
campaign on 18/06/2019.
 
• campaigns: contains information about the different campaigns organized by DSC since 
December 2014.
− campaignID: The unique ID of the campaign.
− date: The date of the campaign (when the letters were sent).
− lettersSent: The number of letters sent.
− CostUnit: The unitary cost of the campaign (Cost of the campaign divided by the number 
of letters sent).
