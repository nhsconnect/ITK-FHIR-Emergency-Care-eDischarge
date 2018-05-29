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
			<th width="18%">Section</th>
			<th width="30%">Description</th>
			<th width="11%">Cardinality</th>
			<th width="11%">MRO*</th>
			<th width="30%">Values</th>
		</tr>
	</thead>
 <tbody>
  <tr>
   <td>Discharge details</td>
   <td>The details of the patient's discharge from hospital.</td>
   <td>1 only</td>
   <td>required</td>
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
   <td>Discharge status</td>
   <td>Patient status on discharge from emergency care.</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>Sent as per the ECDS Emergency Care DischargeStatus code set (SNOMED CT) :</td>
  </tr>
  <tr>
   <td>Date/time of discharge</td>
   <td>The actual date of discharge</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>The date and time of discharge as recorded by the PAS or discharging system.</td>
  </tr>
  <tr>
   <td>Discharge destination</td>
   <td>The destination of the patient on discharge. National codes. Eg, High Dependency Unit.</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>Sent as per the ECDS Emergency Care Discharge Destination code set (SNOMED CT).</td>
  </tr>
 </tbody>
</table>

##  Example Discharge Section ##

<script src="https://gist.github.com/IOPS-DEV/8af6e4182fad6c0ce91e46e6d17563b5.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- [Encounter](workflow_encounter.html)






