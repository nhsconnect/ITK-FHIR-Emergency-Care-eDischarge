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
The Contact for further information section carries information about the contact details. PRSB Elements should be formatted as subheadings in any HTML sent.

<table style="width:100%;max-width: 100%;">
	<thead>
		<tr>
			<th width="15%">Section</th>
			<th width="35%">Description</th>
			<th width="5%">Card.</th>
			<th width="5%">MRO*</th>
			<th width="40%">FHIR Target and Guidance</th>
		</tr>
	</thead>
 <tbody>
  <tr>
   <td>Contact for further information</td>
   <td>Details of a contact who can provide further information.</td>
   <td>1 only</td>
   <td>M</td>
   	<td>Carried in the CodeableConcept of <b>Composition.section.code</b> FHIR element.</td>
  </tr>
		<tr>
			<th>PRSB Element</th>
			<th>Description</th>
			<th>Card.</th>
			<th>MRO*</th>
			<th>FHIR Target and Guidance</th>		
		</tr>
  <tr>
   <td>Contact for further information</td>
   <td>The contact details of whom to contact for information regarding this attendance.</td>
   <td>1 only</td>
   <td>M</td>
   <td>The contact details may be for an individual or team (for example a phone number for the emergency department administrator). Free text.</td>
  </tr>
		<tr>
		<td colspan="5"><b>* M=Mandatory R=Required O=Optional</b></td>
		</tr>
 </tbody>
</table>

##  Example Contact for further information Section ##

<script src="https://gist.github.com/IOPS-DEV/2fc82c41a8105e6cb66b03c59dccdc24.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK3 FHIR Emergency Care eDischarge does not currently support coded contact for further information.






