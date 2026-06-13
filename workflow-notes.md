Workflow Notes

This file explains how I think about lead tracking workflows, data accuracy, and possible failure points.

Workflow Goal

The goal of this workflow is to track real estate leads from different sources, such as project pages, WhatsApp clicks, and paid campaigns.

The main idea is not only to collect the lead, but also to understand where it came from and how the sales team should follow up.

Data Captured

The workflow can capture:

Project name
Phone number
Lead source
Campaign name
UTM parameters
WhatsApp click time
Form submission time

Edge Cases

Some cases need special handling:

The same phone number submits more than once
UTM parameters are missing
A user clicks WhatsApp but does not submit a form
The phone number format is wrong
The database request fails
A lead comes from more than one campaign

Review Notes

Before using this kind of workflow in production, I would check:
Is the phone number validated?
Are duplicate leads handled?
Are failed requests logged?
Is the source saved correctly?
Can the sales team trust the report?
What happens if the campaign data is missing?

Risk

If this workflow is implemented badly, the business may count the same lead twice, assign leads to the wrong source, or make marketing decisions based on wrong data.
