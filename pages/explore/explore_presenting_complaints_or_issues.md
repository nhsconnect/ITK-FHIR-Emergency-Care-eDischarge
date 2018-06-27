---
title: Presenting complaints or issues Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_presenting_complaints_or_issues.html
summary: "Gives information about the Presenting complaints or issues section"
---

{% include custom/section.warnbanner.html %}

## Presenting Complaints Or Issues Section Content##
The Presenting complaints or issues section carries information about the complaints or issues experienced by the patient. Elements should be formatted as subheadings in any HTML sent.

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
   <td>Presenting complaints or issues</td>
   <td>The description of the health problems and issues experienced by the patient resulting in their attendance.</td>
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
   <td>Presenting complaints or issue</td>
   <td>The list and description of the health problems and issues experienced by the patient resulting in the attendance. This may include disease state, medical condition, response and reaction to therapies, eg blackout, dizziness, chest pain, follow-up from admission, falls, a specific procedure, investigation or treatment.</td>
   <td>1 only</td>
   <td>M</td>
   <td>Only ONE (chief complaint) sent as per the ECDS Emergency Care Chief Complaint code set (SNOMED CT).Text and if available a SNOMED CT concept carried in the CodeableConcept of the <b>Condition.code</b> FHIR element.</td>
  </tr>
		<tr>
		<td colspan="5"><b>* M=Mandatory R=Required O=Optional</b></td>
		</tr>
 </tbody>
</table>

## Example Presenting Complaints Or Issues Section ##

<script src="https://gist.github.com/IOPS-DEV/cec203cc480ab3a7977f281c68d96461.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK3 FHIR Emergency Care eDischarge does not currently support coded presenting complaints or issues information.






