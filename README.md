# Real Estate Lead Tracking Workflow

This repository explains a simple lead tracking workflow I worked on for real estate campaigns and WhatsApp clicks.

## Problem

Leads were coming from different sources such as project pages, WhatsApp clicks, and paid campaigns. The sales team could receive the lead, but they did not always know which campaign or project generated it.

## Tools

- JavaScript
- PHP
- SQL
- UTM tracking

## Workflow

When a user submits a form or clicks WhatsApp, the system captures:

- Project name
- Phone number
- Lead source
- Campaign name
- Time of action

The data is then saved and shown inside a CRM-style dashboard for follow-up.

## Edge Cases

- Duplicate phone numbers
- Missing UTM parameters
- Wrong phone format
- WhatsApp clicks without form submission
- Failed database requests

## Why it matters

If this workflow is not handled correctly, the same lead can be counted more than once, or a campaign can look weaker than it really is because the source was not saved correctly.
