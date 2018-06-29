---
title: Person Completing Record Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_per_com_record.html
summary: "Gives information about the Person completing record section"
---

{% include custom/section.warnbanner.html %}

## Person Completing Record Section Content##
The Person completing record section carries information about the person who completed the record. Elements should be formatted as subheadings in any HTML sent.


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
			<td>Person completing record</td>
			<td>The details of the person who filled out the record.</td>
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
			<td>Name</td>
			<td>The name of the person completing the record, preferably in a structured format.</td>
			<td>1 only</td>
			<td>M</td>
			<td>The person name as held on the source system. Where possible this should be broken down into its constituent parts (prefix, given name, family name, and suffix) within the text and carried in the FHIR element <b>Practitioner.name</b> . An identifier for the person completing the record will be sent in the FHIR element <b>Practitioner.identifier</b>.</td>
		</tr>
		<tr>
			<td>Professional identifier</td>
			<td>Professional identifier for the person completing the record e.g., GMC number, HCPC number etc or the personal identifier used by the local organisation.</td>
			<td>0 to 1</td>
			<td>R</td>
			<td>The professional identifier type and the identifier itself of the person completing the record held on the source system which <b>MUST NOT</b> be in text but carried in the FHIR element <b>Practitioner.identifier</b> and <b>Practitioner.identifier.type</b>.</td>
		</tr>
		<tr>
		<td colspan="5"><b>* M=Mandatory R=Required O=Optional</b></td>
		</tr>
	</tbody>
</table>

## Example Person Completing Record Section ##

<script src="https://gist.github.com/IOPS-DEV/4eceababbca389067cde4aefd2d61cde.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK3 FHIR Emergency Care eDischarge does not currently support coded Person completing record information.






