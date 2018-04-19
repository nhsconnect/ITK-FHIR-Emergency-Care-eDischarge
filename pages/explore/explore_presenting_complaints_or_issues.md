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
The Presenting complaints or issues section carries information about the complaints or issues experienced by the patient. Elements should be formatted as sub headings in any html sent.

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
   <td>Presenting complaints or issues</td>
   <td>The description of the health problems and issues experienced by the patient resulting in their attendance.</td>
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
   <td>Presenting complaints or issue</td>
   <td>The list and description of the health problems and issues experienced by the patient resulting in the attendance. This may include disease state, medical condition, response and reaction to therapies, eg blackout, dizziness, chest pain, follow-up from admission, falls, a specific procedure, investigation or treatment.</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>Only ONE (chief complaint) sent as per the ECDS Emergency Care Chief Complaint code set (SNOMED CT).</td>
  </tr>
 </tbody>
</table>

## Example Presenting Complaints Or Issues Section ##

<script src="https://gist.github.com/IOPS-DEV/cec203cc480ab3a7977f281c68d96461.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK FHIR Emergency Care eDischarge does not currently support coded presenting complaints or issues information.






