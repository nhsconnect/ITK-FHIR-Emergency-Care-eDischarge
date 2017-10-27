---
title: Senior reviewing clinician Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_senior_reviewing_clinician.html
summary: "Gives information about the Senior reviewing clinician section"
---

{% include custom/section.warnbanner.html %}

## Senior Reviewing Clinician Section Content##
The Senior reviewing clinician section carries information about the senior reviewing clinician, items in bold are subheadings and should be formatted as such in any html sent:

- **Name** - The name of the senior clinician responsible for reviewing the patient treatment and discharge plan. The person name as held on the source system.  Where possible this should be broken down into its constituent parts (prefix, given name, family name, suffix).
- **Professional identifier** - The unique identifier issued by the regulatory body, e.g. GMC number, HCPC number etc...  The professional identifier type (professional registration issuer code) and the identifier (professional registration entry identifier) itself as held on the source system.  An identifier for the person completing the record will be sent (but may not be displayed in the rendered message).

##  Example Senior Reviewing Clinician Section ##

<script src="https://gist.github.com/IOPS-DEV/a9d7ecd57c3b92d3eb3629e8c4d73e46.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK FHIR eDischarge Emergency Care does not currently support coded Senior reviewing clinician information.






