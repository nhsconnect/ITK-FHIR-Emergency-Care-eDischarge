---
title: Clinical Narrative Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_clinical_narrative.html
summary: "Gives information about the Clinical narrative section"
---

{% include custom/section.warnbanner.html %}

## Clinical Narrative Section Content ##
The Clinical narrative section carries details of the clinical narrative. Where possible, very brief,subheadings should be formatted as such in any html sent:

<table width="100%">
<tr>
<th width="25%">Sub-section</th>
<th width="45%">Description</th>
<th width="15%">Cardinally</th>
<th width="15%">Conformance</th>
</tr>
<tr>
<td>Clinical narrative</td>
<td>A description detailing a patient’s reason for attendance and results from the diagnostic and treatment process.</td>
<td>1..1</td>
<td>Mandatory</td>
</tr>
</table> 

##  Example Clinical Narrative Section ##

<script src="https://gist.github.com/IOPS-DEV/f90f3d0e728470d48de1c41ad08fdfab.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK FHIR Emergency Care eDischarge does not currently support a coded clinical narrative.






