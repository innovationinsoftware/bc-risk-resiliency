# Exercise 2b: BIA for a Bank

A Business Impact Analysis (BIA) identifies how a disruption affects business operations and helps prioritize which processes must be recovered first

BIA bridges the gap between technical risk analysis and resilience planning, like creating redundant services or backing up data, and business-level continuity planning.

The goals of this exercise are to:
- Get you familiar with the basic flow of an BIA
- Get you used to framing the sorts of questions you should be asking during a BIA to guide your investigation

## Scenario

- You are part of the IT Risk and Resilience team for FinServe Bank, a mid-sized financial services company
- FinServe relies on several IT systems to support its operations
- Over the past year, the bank has had several short service interruptions
- YOu have been tasked to lead a formal BIA to guide investment in resilience with respect to service outages


## Background

- Regulators have cautioned the bank that there has been an increase in customer complaints of services being down at FinServe and would like an initial formal report on mitigation steps being taken to address the issues
- Senior management is concerned that these interruptions may indicate problems within the IT department at the bank and have the potential to escalate into longer disruptions that would cause lasting harm to ghe banks market share and reputation, as well as resulting in potential regulatory fines
- The bank's IT environment is mixture of legacy technology deployed in the 1990s and newer technologies

## Business Operations

- For this exercise, these are the business operations at the bank that are the focus of the BIA for service outages
- **Online Banking**
  - Customer portal for account access, transfers, bill payments
  - Tech stack: Web servers, databases, payment gateway
- **Loan Processing**	
  - Internal system for loan approvals
  - Tech stack: Application servers, database, document store
- **Customer Support**	
  - Call center operations	
  - Tech stack: VoIP, CRM, email
- **Payroll & HR** 
  - Staff payments, benefits, compliance	
  - Tech stack: ERP (Enterprise Resource Planning) system, database
- **Trading Platform**	
  - Real-time trading system	
  - Tech stack: Market data feeds, high-speed compute nodes


## Step 1: Identify Critical Business Functions

- Which processes, if disrupted, would stop or severely impact business operations?
- Can you describe what the impact would be?
- What sort of data would you need to collect to make your assessment?

## Step 2: Identify Dependencies

- For each business function, identify the supporting IT systems, data, and third-party dependencies
  - Also identify what sort of steps you would take to ensure your identification of IT support systems is accurate 
- What technology or vendor failures would make this function unavailable?

### Analysis by example
- A tool for identifying which resources are involved in a business process is scenario analysis
- Take an example of a typical unit of work like a customer paying their electric bill or an inquiry handled by the call center 
- Follow that unit of work through the business process
- At each step, which technology would be used at that step
- If there are a variety of types of transactions, use a representative sample of each
  - For a more detailed analysis, look at the "what if?" variants, for example, a payment fails because there is a hold on the customer's account.  

## Step 3: Assess the Impact of Downtime

- For each of the business processes identified, identify the impact over time based on the following risk categories
  - **Financial**: revenue loss, fees/penalties, trading P&L, cost of manual work
  - **Customer**: number of customers unable to transact, VIP/segment impact, queue/abandon rates
  - **Regulatory & Legal:** reportable incidents, filing deadlines missed, consent order exposure, fines
  - **Operational**: throughput drop, backlog growth, staff hours for workaround, dependency breakage
  - **Reputation**: media/social escalation, complaints, net promoter score drop, executive attention
- Use the ranking of high/medium/low for impact
- And assess the impact over the following time periods
  - 1 hour
  - 4 hours
  - 1 day
  - 3 days
  - And an overall prioritization
- How does the impact escalate over time? Which functions become critical fastest?

## Step 4: Define RTO and RPO

- Determine Recovery Time Objective (RTO), how quickly a service must be restored
- Determine Recovery Point Objective (RPO), how much data loss is acceptable
- What data would you need to determine these?
- For example, if the system fails at 3 PM, by when must it be restored to avoid serious impact?

## Step 5: Prioritize Recovery

- Rank functions from most critical to least critical, based on their overall impact and RTO.
- Which systems need real-time replication, and which can tolerate delays or manual fallback?

## Step 6: Link to Risk Mapping

- Which high-risk areas affect the most critical business functions?
- Which process improvements (e.g., patching, backup testing, access control) would improve resilience for these functions?






