---
title: Attendance details section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_attendance_details.html
summary: "Gives information about the Attendance details section"
---

{% include custom/section.warnbanner.html %}

## Attendance Details Section Content ##
The Attendance details section carries information about Attendance details used. Elements should be formatted as sub headings in any HTML sent.


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
   <td>Attendance details</td>
   <td>The details of the patient contact.</td>
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
   <td>Date and time of contact</td>
   <td>Date and time of the appointment, contact or attendance.</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>The date as recorded on the PAS</td>
  </tr>
 </tbody>
</table>


## Example Attendance details Section ##

<script src="https://gist.github.com/IOPS-DEV/267964b88b286590ec7a33d6cb678c04.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK FHIR Emergency Care eDischarge does not currently support coded attendance details.






