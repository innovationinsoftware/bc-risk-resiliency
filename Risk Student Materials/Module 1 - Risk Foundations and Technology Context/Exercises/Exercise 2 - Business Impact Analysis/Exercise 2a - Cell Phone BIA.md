# Exercise 2a: Cell Phone BIA

This is a warm-up exercise to introduce the methodology of a BIA

This exercise will focus on the processes that your cell phone provides.

## Step 1: Identify Critical Business Functions

- Take a moment to look at the various "business functions" you cell phone provides
- For example:
  - Banking and payments
  - Scheduling - keeping track of appointments and responsibilities
  - Information support - using tools like maps, web searches, review sites, etc.
- For the purposes of this exercise, we are only interested in the role your phone plays in helping you to do the things that are critical to your "getting things done"

- Identify the three most important (to you) function your phone provides
- Which processes, if disrupted, would stop or severely impact you?

## Step 2: Identify Dependencies

- For each of those functions, identify the dependencies
  - Your phone
  - Cell provider
  - Third party apps
  - Other services accessed
- What technology or vendor failures would make this function unavailable?

## Step 3: Assess the Impact of Downtime

- Estimate the impact over time (e.g., 1 hour, 4 hours, 1 day, 3 days).
- Use a qualitative ranking (High/Medium/Low)

## Step 4: Define RTO and RPO
- Determine Recovery Time Objective (RTO)
  - How quickly a service must be restored
- Determine Recovery Point Objective (RPO)
  - How much data loss is acceptable
- If the system fails at 3 PM, by when must it be restored to avoid serious impact?

## Step 5: Prioritize Recovery
- Rank functions from most critical to least critical, based on their overall impact and RTO.

## Step 6: Controls and Resilience
- For of the processes you defined, what sort of risk controls could you implement to mitigate the disruption?
- What sort of recovery plan could you implement to recover from each of the failures you identified?


