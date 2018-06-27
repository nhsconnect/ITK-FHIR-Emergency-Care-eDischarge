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
The Discharge details section carries details of the patient's discharge. Elements should be formatted as subheadings in any HTML sent.

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
			<td>Discharge details</td>
			<td>The details of the patient's discharge from hospital.</td>
			<td></td>
			<td>R</td>
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
   <td>Discharge status</td>
   <td>Patient status on discharge from emergency care.</td>
   <td>1 only</td>
   <td>M</td>
   <td>This is sent as text and and "MUST" be included in the FHIR element <b>Encounter.extension(emergencyCareDischargeStatus)</b> and will contain a code from the SNOMED Clinical Terminology UK coding system that describes the status of the Patient on discharge from an Emergency Care Department. Captures whether treatment took place within the ED, if the patient was streamed to another service or if the patient left before treatment was complete. Any code from the SNOMED CT UK 'Emergency care discharge status' subset with subset original id 75041000000135; the corresponding SNOMED CT UK Refset fully specified name is 'Emergency care discharge status simple reference set (foundation metadata concept)' with Refset Id 999003021000000104. </td>
  </tr>
		<tr>
			<td>Date/time of discharge</td>
			<td>The actual date of discharge</td>
			<td>1 only</td>
			<td>M</td>
			<td>Text indicating date and time of discharge as recorded by the PAS or discharging system. This <b>SHOULD</b> also be carried in the FHIR element <b>Encounter.period.end</b>.</td>
		</tr>
  <tr>
   <td>Discharge destination</td>
   <td>The destination of the patient on discharge. National codes. Eg, High Dependency Unit.</td>
   <td>1 only</td>
   <td>M</td>
   <td>Text and coded using a value from the ECDS Emergency Care Discharge Destination subset (SNOMED CT) with original subset ID of 75031000000130 which is carried in the CodeableConcept of the FHIR element <b>Encounter.hospitalization.dischargeDisposition</b>.</td>
  </tr>
	<tr>
	<td colspan="5"><b>* M=Mandatory R=Required O=Optional</b></td>
	</tr>
 </tbody>
</table>

##  Example Discharge Section ##

<script src="https://gist.github.com/IOPS-DEV/8af6e4182fad6c0ce91e46e6d17563b5.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- [Encounter](workflow_encounter.html)






