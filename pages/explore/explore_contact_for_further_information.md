---
title:  Contact for further information Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_contact_for_further_information.html
summary: "Gives information about the Contact for further information section"
---

{% include custom/section.warnbanner.html %}

## Contact for further information Content ##
The Contact for further information section carries information about the contact details, subheadings should be formatted as such in any html sent:

<table width="100%">
<tr>
<th width="25%">Sub-section</th>
<th width="45%">Description</th>
<th width="15%">Cardinally</th>
<th width="15%">Conformance</th>
</tr>
<tr>
<td>Contact for further information</td>
<td>The contact details of whom to contact for information regarding this attendance.  E.g. The contact details may be for an individual or team (for example a phone number for the emergency department administrator). This is free text</td>
<td>1..1</td>
<td>Mandatory</td>
</tr>
</table> 


##  Example Contact for further information Section ##

<script src="https://gist.github.com/IOPS-DEV/2fc82c41a8105e6cb66b03c59dccdc24.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK FHIR Emergency Care eDischarge does not currently support coded contact for further information.






