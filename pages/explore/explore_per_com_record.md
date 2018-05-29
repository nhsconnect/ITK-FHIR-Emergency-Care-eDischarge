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
			<th width="18%">Section</th>
			<th width="30%">Description</th>
			<th width="11%">Cardinality</th>
			<th width="11%">MRO*</th>
			<th width="30%">Values</th>
		</tr>
	</thead>
 <tbody>
  <tr>
   <td>Person completing record</td>
   <td>The details of the person who filled out the record.</td>
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
   <td>Name</td>
   <td>The name of the person completing the record, preferably in a structured format.</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>The person name as held on the source system. Where possible this should be broken down into its constituent parts (prefix, given name, family name, and suffix).</td>
  </tr>
  <tr>
   <td>Professional identifier</td>
   <td>Professional identifier for the person completing the record e.g., GMC number, HCPC number etc or the personal identifier used by the local organisation.</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>The professional identifier type and the identifier itself as held on the source system. <a href="http://www.datadictionary.nhs.uk/data_dictionary/data_field_notes/p/prod/professional_registration_issuer_code_de.asp?shownav=1"/><professional registration issuer code <a href="http://www.datadictionary.nhs.uk/data_dictionary/data_field_notes/p/prod/professional_registration_entry_identifier_de.asp?shownav=1"/>
   professional registration entry identifier. An identifier for the person completing the record will be sent (but may not be displayed in the rendered message).</td>
  </tr>
 </tbody>
</table>


## Example Person Completing Record Section ##

<script src="https://gist.github.com/IOPS-DEV/979484d91e5ab8e5c9f1c4edf85404b5.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK3 FHIR Emergency Care eDischarge does not currently support coded Person completing record information.






