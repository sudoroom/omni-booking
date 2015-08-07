# omni-booking
booking system for the omni commons

The Omni Commons regularly hosts events in the space, but our current booking system leaves a lot to be desired. Let's build a better one that could be easily forked and replicated in other collective spaces!

To see the current booking system and calendar, follow the following links:
* https://omnicommons.org/occupy
* https://omnicommons.org/calendar

## Features
* a step-by-step wizard for submitting an event request
* automated checking of Omni's calendar for time/date/location conflicts 
* a backend for reviewing and confirming/rejecting an event proposal
* upon confirmation, automatically populating Omni's calendar with the event
* upon confirmation, a step-by-step wizard for e-signing a contract, paying the invoice, and displaying any additional deposit or insurance requirements

## Detailed UX Flow
* See here for our current process: https://omnicommons.org/occupy
* Scenario: Someone wants to book a series of dance rehearsals in the Disco Room leading up to a performance in the ballroom. They've never been to Omni before.
* They visit https://omnicommons.org and click a link (currently doesn't exist) to book an event
* The Booking site could be a wizard that guides people through our policies and fee structure:
* Pg.1: Rental Policy & Fee Structure: https://omnicommons.org/occupy/omni-commons-rental-policy-and-fee-structure/
* Pg 2: Rules for the Omni Commons: https://omnicommons.org/wiki/Rules (needs to be expanded)
* Pg 3: Your Contact Info: Name, Email, Your Organization, Relationship to Omni, Omni Point Person (optional), Sponsoring Group (optional)
* Pg 4: When & Where: Date, Time, Location (this could be visualized with thumbnail images of each rentable space in the building that link to a wiki page with full-size images and/or links to a 3D photo of the space), Recurrence (if any), Attendance, Amplified Sound (y/n), Needs Quiet (y/n)
* When selecting a date/time/location, it would be great if the calendar could be checked for any conflicts ''extra nice-to-have!!''
* Pg 5: Describe in Detail: Event Name, Public Description, Private Details (note to Commons Working Group organizers), Who is welcome? (public/private), Admission Cost, "Our costs are roughly $20,000/month. What are you able to pay for use of the space?", Do you plan to serve alcohol? (y/n), Do you plan to sell alcohol? (y/n)
* After completing the wizard, the form is sent to booking@lists.omnicommons.org and the event organizer receives a confirmation of receipt in their inbox saying that they will receive a reply by the Second Saturday of the month (deadline to submit is Second Fridays of the month for a reservation within the next month)
* Commons Working Group members can log into the backend and review requests. If an event proposal is accepted, the following occurs: 
1. The event is posted to the Omni calendar under the category "Others' Events", 
2. The event organizer receives an email requesting they follow a link to another wizard that guides them through e-signing a contract, payment, deposit requirements (if any), and insurance requirements (if any)
* Event Contract (short for simple events): https://omnicommons.org/cloud/index.php/s/ADLrv1BcyR65AfN
* Event Contract (long for events with >50 attendees, loud music, and/or presence of alcohol): https://omnicommons.org/cloud/index.php/s/6nQMDIAPmK5st08
* Invoice & Payment: Can be integrated with either Stripe or Quickbooks (both of which do invoicing. Quickbooks is what's being used currently. It would be nice to have Quickbooks set up on Omni's server)
* Insurance Requirements: Can use this flowchart to determine what kind of insurance is needed: https://drive.google.com/file/d/0ByjR12L1MEjCRXhiMU04aFN6OXc/view
* Ideally, event organizers should have access to their event alone in the case they wish to change their event's title or description
