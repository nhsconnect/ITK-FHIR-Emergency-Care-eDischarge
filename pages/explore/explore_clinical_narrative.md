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
The Clinical narrative section carries details of the clinical narrative. Where possible, very brief. Elements should be formatted as sub headings in any HTML sent.

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
   <td>Clinical narrative</td>
   <td>A brief description of the encounter.</td>
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
   <td>Clinical narrative</td>
   <td>A description detailing a patient's reason for attendance, results from the diagnostic and treatment process.</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>Free text.</td>
  </tr>
 </tbody>
</table>

##  Example Clinical Narrative Section ##

<script src="https://gist.github.com/IOPS-DEV/f90f3d0e728470d48de1c41ad08fdfab.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK FHIR Emergency Care eDischarge does not currently support a coded clinical narrative.






