---
title: Discharge Details Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_discharge_details.html
summary: "Gives information about the Discharge details section"
---

{% include custom/section.warnbanner.html %}

## Discharge Details Section Content##
The Discharge details section carries details of the patient's discharge, subheadings should be formatted as such in any html sent:

<table width="100%">
<tr>
<th width="25%">Sub-section</th>
<th width="45%">Description</th>
<th width="15%">Cardinally</th>
<th width="15%">Conformance</th>
</tr>
<tr>
<td>Discharge destination</td>
<td>The destination of the patient on discharge. National codes. Eg, High Dependency Unit.
</td>
<td>1..1</td>
<td>Mandatory</td>
</tr>
<tr>
<td>Discharge status</td>
<td>Patient status on discharge from emergency care. Sent as per the ECDS Emergency Care Discharge
Status code set (SNOMED CT):</td>
<td>1..1</td>
<td>Mandatory</td>
</tr>
<tr>
<td>Date/time of discharge</td>
<td>The actual date of discharge</td>
<td>1..1</td>
<td>Mandatory</td>
</tr>
</table>

##  Example Discharge Section ##

<script src="https://gist.github.com/IOPS-DEV/8af6e4182fad6c0ce91e46e6d17563b5.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- [Encounter](workflow_encounter.html)






