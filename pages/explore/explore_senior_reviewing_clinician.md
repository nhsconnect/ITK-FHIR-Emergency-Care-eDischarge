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
The Senior reviewing clinician section carries information about the senior reviewing clinician. Elements should be formatted as subheadings in any HTML sent.

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
   <td>Senior reviewing clinician</td>
   <td>The details of the senior clinician who reviewed the record.</td>
   <td>0 to 1</td>
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
   <td>Name</td>
   <td>The name of the senior clinician responsible for reviewing the patient treatment and discharge plan.</td>
   <td>1 only</td>
   <td>M</td>
   <td>The person name as held on the source system. Where possible this should be broken down into its constituent parts (prefix, given name, family name, suffix). The is carried in text and in the FHIR element <b>Practitioner.name</b> and associated sub-elements.</td>
  </tr>
  <tr>
   <td>Professional identifier</td>
   <td>The unique identifier issued by the regulatory body e.g., GMC number, HCPC number etc.</td>
   <td>0 to 1</td>
   <td>R</td>
   <td>The professional identifier type and the identifier itself as held on the source system. This is an identifier for the person completing the record will be sent (but may not be displayed in the rendered message). This <b>MUST NOT</b> be sent in text but carried in the FHIR element <b>Practitioner.identifier</b> and <b>Practitioner.identifier.type</b></td>
  </tr>
		<tr>
		<td colspan="5"><b>* M=Mandatory R=Required O=Optional</b></td>
		</tr>
 </tbody>
</table>

##  Example Senior Reviewing Clinician Section ##

<script src="https://gist.github.com/IOPS-DEV/a9d7ecd57c3b92d3eb3629e8c4d73e46.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK3 FHIR Emergency Care eDischarge  does not currently support coded senior reviewing clinician information.






