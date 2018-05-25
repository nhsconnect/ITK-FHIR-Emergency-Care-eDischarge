---
title: Emergency Care eDischarge Headings
keywords:  messaging
tags: [fhir,messaging]
sidebar: foundations_sidebar
permalink: explore_headings.html
summary: "Overview of the Emergency Care eDischarge headings"
---

{% include custom/search.warnbanner.html %}
{% include custom/section.warnbanner.html %}

## Overview ##

This section provides a list of the PRSB headings used for text sections in the ITK FHIR Emergency Care eDischarge based on the "Standards for the clinical structure and content of patient records" documentation. 

This section lists the following

- The headings used
- An overview of the type of information carried within the text section
- An example of a text section instance
- A list of the coded resources which may be used to give the text carried in the section in a coded format. 
 
## Typical Text Section Content ##
This diagram shows the elements of a typical text section which is found in the FHIR Composition Resource.
Note: the examples of section HTML in this specification show only example HTML format such as tables. This is an exemplar format. There is no mandated format for the section HTML. 

<img src="images/explore/section_description.png" style="width:90%;max-width: 90%;"/>
 
## Headings Used By Emergency Care eDischarge ##

<table>
	<tr>
		<th width="40%">Section Name</th>
		<th width="20%">SNOMED Concept</th>
		<th width="13%">Cardinally</th>
		<th width="13%">Conformance</th>
		<th width="13%">Associated Coded Profiles</th>
	</tr>
	<tr>
		<td>
			<a href="explore_allergies_and_adverse_reactions.html">Allergies and adverse reactions</a>
		</td>
		<td>886921000000105</td>
		<td>1..1</td>
		<td>Required</td>
		<td>2</td>
	</tr>
	<tr>
		<td>
			<a href="explore_attendance_details.html">Attendance details</a>
		</td>
		<td>1077881000000105</td>
		<td>1..1</td>
		<td>Mandatory</td>
		<td>O</td>
	</tr>
	<tr>
		<td>
			<a href="explore_clinical_narrative.html">Clinical narrative</a>
		</td>
		<td>1077901000000108</td>
		<td>1..1</td>
		<td>Mandatory</td>
		<td>0</td>
	</tr>
	<tr>
		<td>
			<a href="explore_contact_for_further_information.html">Contact for further information</a>
		</td>
		<td>1077931000000102</td>
		<td>1..1</td>
		<td>Mandatory</td>
		<td>0</td>
	</tr>
	<tr>
		<td>
			<a href="explore_diagnoses.html">Diagnoses</a>
		</td>
		<td>887161000000102</td>
		<td>0..1</td>
		<td>Required</td>
		<td>2</td>
	</tr>
	<tr>
		<td>
			<a href="explore_discharge_details.html">Discharge details</a>
		</td>
		<td>886811000000106</td>
		<td>1..1</td>
		<td>Required</td>
		<td>1</td>
	</tr>
	<tr>
		<td>
			<a href="explore_distribution_list.html">Distribution list</a>
		</td>
		<td>887261000000109</td>
    	<td>1..1</td>
		<td>Mandatory</td>
		<td>4</td>
	</tr>
	<tr>
		<td>
			<a href="explore_gp_practice.html">GP practice</a>
		</td>
		<td>886711000000101</td>
    	<td>1..1</td>
		<td>Mandatory</td>
		<td>2</td>
	</tr>
	<tr>
		<td>
			<a href="explore_information_given.html">Information and advice given</a>
		</td>
		<td>1052951000000105</td>
		<td>0..1</td>
		<td>Required</td>
		<td>0</td>
	</tr>
	<tr>
		<td>
			<a href="explore_legal_info.html">Legal information</a>
		</td>
		<td>886961000000102</td>
		<td>0..1</td>
		<td>Required</td>
		<td>0</td>
	</tr>
	<tr>
		<td>
			<a href="explore_medication.html">Medications and medical devices</a>
		</td>
		<td>933361000000108</td>
		<td>0..1</td>
		<td>Optional</td>
		<td>2</td>
	</tr>
	<tr>
		<td>
			<a href="explore_patient_demographics.html">Patient demographics</a>
		</td>
		<td>886731000000109</td>
    	<td>1..1</td>
		<td>Mandatory</td>
		<td>1</td>
	</tr>
	<tr>
		<td>
			<a href="explore_per_com_record.html">Person completing record</a>
		</td>
		<td>887231000000104</td>
		<td>1..1</td>
		<td>Mandatory</td>
		<td>0</td>
	</tr>
	<tr>
		<td>
			<a href="explore_plan_req_actions.html">Plan and requested actions</a>
		</td>
		<td>887201000000105</td>
		<td>1..1</td>
		<td>Mandatory</td>
		<td>0</td>
	</tr>
	<tr>
		<td>
			<a href="explore_presenting_complaints_or_issues.html">Presenting complaints or issues</a>
		</td>
		<td>886891000000102</td>
		<td>1..1</td>
		<td>Mandatory</td>
		<td>2</td>
	</tr>
	<tr>
		<td>
			<a href="explore_procedures.html">Procedures</a>
		</td>
		<td>887171000000109</td>
		<td>0..1</td>
		<td>Required</td>
		<td>2</td>
	</tr>
	<tr>
		<td>
			<a href="explore_referrer.html">Referrer details</a>
		</td>
		<td>1052891000000108</td>
		<td>0..1</td>
		<td>Required</td>
		<td>0</td>
	</tr>
	<tr>
		<td>
			<a href="explore_safety_alerts.html">Safety alerts</a>
		</td>
		<td>886931000000107</td>
		<td>0..1</td>
		<td>Required</td>
		<td>0</td>
	</tr>
	<tr>
		<td>
			<a href="explore_safeguarding.html">Safeguarding</a>
		</td>
		<td>886931000000107</td>
		<td>0..1</td>
		<td>Required</td>
		<td>0</td>
	</tr>
	<tr>
		<td>
			<a href="explore_social_context.html">Senior reviewing clinician</a>
		</td>
		<td>1078901000000109</td>
		<td>0..1</td>
		<td>Required</td>
		<td>0</td>
	</tr>
</table>


## Overview of Emergency Care eDischarge Sections and Coded profiles ##
This diagram illustrates the sections used in Emergency Care eDischarge and which sections allow coded representation of the section text. 


<a href="images/explore/EC_composition_overview.png" target="_blank" style="width: 100%;max-width: 100%;"><b>Click to open in new window</b></a>


<img src="images/explore/EC_composition_overview.png" style="width:auto;height: auto;"/>



The text sections are carried in the FHIR composition resource. 
This is profiled as the [ITK-EC-Compostion](https://fhir.nhs.uk/STU3/StructureDefinition/ITK-EC-Composition-1)





