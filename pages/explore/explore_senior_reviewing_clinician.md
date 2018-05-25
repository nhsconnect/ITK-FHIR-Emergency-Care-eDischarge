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
The Senior reviewing clinician section carries information about the senior reviewing clinician. Elements should be formatted as sub headings in any HTML sent.

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
   <td>Senior reviewing clinician</td>
   <td>The details of the senior clinician who reviewed the record.</td>
   <td>0 to 1</td>
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
   <td>Name</td>
   <td>The name of the senior clinician responsible for reviewing the patient treatment and discharge plan.</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>The person name as held on the source system. Where possible this should be broken down into its constituent parts (prefix, given name, family name, suffix).</td>
  </tr>
  <tr>
   <td>Professional identifier</td>
   <td>The unique identifier issued by the regulatory body e.g., GMC number, HCPC number etc.</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>The professional identifier type and the identifier itself as held on the source system. An identifier for the person completing the record will be sent (but may not be displayed in the rendered message).</td>
  </tr>
 </tbody>
</table>

##  Example Senior Reviewing Clinician Section ##

<script src="https://gist.github.com/IOPS-DEV/a9d7ecd57c3b92d3eb3629e8c4d73e46.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK FHIR Emergency Care eDischarge  does not currently support coded senior reviewing clinician information.






