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
The Clinical narrative section carries details of the clinical narrative. Where possible, very brief. Elements should be formatted as subheadings in any HTML sent.

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
   <td>Clinical narrative</td>
   <td>A brief description of the encounter.</td>
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
   <td>Clinical narrative</td>
   <td>A description detailing a patient's reason for attendance, results from the diagnostic and treatment process.</td>
   <td>1 only</td>
   <td>M</td>
   <td>Free text.</td>
  </tr>
		<tr>
		<td colspan="5"><b>* M=Mandatory R=Required O=Optional</b></td>
		</tr>
 </tbody>
</table>

##  Example Clinical Narrative Section ##

<script src="https://gist.github.com/IOPS-DEV/f90f3d0e728470d48de1c41ad08fdfab.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK3 FHIR Emergency Care eDischarge does not currently support a coded clinical narrative.






