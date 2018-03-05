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
The Contact for further information section carries information about the contact details. Elements should be formatted as sub headings in any html sent.

<table style="width:100%;max-width: 100%;">
	<thead>
		<tr>
			<th width="18%">Section</th>
			<th width="30%">Description</th>
			<th width="11%">Cardinality</th>
			<th width="11%">MRO*</th>
			<th width="30%">Values</th>
		</tr>
	</thead>
 <tbody>
  <tr>
   <td>Contact for further information</td>
   <td>Details of a contact who can provide further information.</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>&nbsp;</td>
  </tr>
		<tr>
			<th>Element</th>
			<th>Description</th>
			<th>Cardinality</th>
			<th>MRO*</th>
			<th>Values</th>
		</tr>
  <tr>
   <td>Contact for further information</td>
   <td>The contact details of whom to contact for information regarding this attendance.</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>The contact details may be for an individual or team (for example a phone number for the emergency department administrator). Free text.</td>
  </tr>
 </tbody>
</table>

##  Example Contact for further information Section ##

<script src="https://gist.github.com/IOPS-DEV/2fc82c41a8105e6cb66b03c59dccdc24.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK FHIR Emergency Care eDischarge does not currently support coded contact for further information.






