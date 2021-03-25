---
title: Emergency Care eDischarge Headings
keywords:  messaging
tags: [fhir,messaging]
sidebar: foundations_sidebar
permalink: explore_headings.html
summary: "Overview of the Emergency Care eDischarge headings"
---


{% include custom/section.warnbanner.html %}

## Overview ##

This section provides a list of the PRSB headings used for text sections in the ITK3 FHIR Emergency Care eDischarge based on the "Standards for the clinical structure and content of patient records" documentation. 

This section lists the following

- The headings used
- An overview of the type of information carried within the text section
- An example of a text section instance
- A list of the coded resources which may be used to give the text carried in the section in a coded format. 
 
## Typical Text Section Content ##
This diagram shows the elements of a typical text section which is found in the FHIR Composition Resource.
Note: the examples of section HTML in this specification show only example HTML format such as tables. This is an exemplar format. There is no mandated format for the section HTML. 

<img src="images/explore/section_description.png" style="width:90%;max-width: 90%;"/>

## Must Support Property ##
Some elements in the the Composition Resource used within ITK3 Transfer of Care documents have the must support property set to "true"
These are :
- Composition.extension(careSettingTypeExtension)
- Composition.identifier
- Composition.status
- Composition.type
- Composition.subject
- Composition.encounter
- Composition.date
- Composition.author
- Composition.title
- Composition.custodian
- Composition.relatesTo
- Composition.section(slice) Where slice=The PRSB headings for the ITK3 Transfer of Care document type.

The “must support” property has been added to all the elements that must be supported regardless of cardinality.  Whether the conformance of the element is mandatory or optional has no relevance for the “must support” property. This means that for sending or receiving systems to claim conformance to any ITK3 Transfer of Care Composition Profile the following MUST be true:

- The sending system MUST support the creation and sending of all the elements in the list above.
- The sending system MUST support the creation and sending of all Composition.section slices with the specified sub-elements and narrative.* See Note 1. 
- The receiving system MUST support the processing of all the elements in the list above.  
- The receiving system MUST support the display of all Composition.section slices with the specified sub-elements and narrative.

**Note 1** - There are rules around when sections are sent or not sent in a document. These are specified in the document headings sections.

## Population of Correspondence Document Type values ##

Implementers are advised to populate the Correspondence Document Type values for all eDischarge use cases with the following member of the SNOMED Record composition type simple reference set (1127551000000109). 

  - Discharge summary (preferred term) and 373942005 (ref. component ID)

Implementers can choose the most appropriate option when selecting a correspondence care setting member from the Correspondence Care Setting type simple reference set (999000381000000107).  
The title (of the document) held in the Composition profile should be formed from a concatenation of the human readable value for the Correspondence Care Setting and Correspondence Document Type. If a sender organisation wishes to deviate from this approach they should first discuss this with NHS Digital.  
For illustration, the [coded example](https://developer.nhs.uk/apis/itk3emergencycareedischarge-2-8-0/engage_richard_smith.html) provided is already compliant with the outlined approach.
 
## Headings Used By Emergency Care eDischarge ##

<table>
	<tr>
		<th width="40%">Section Name</th>
		<th width="20%">SNOMED Concept</th>
		<th width="13%">Cardinality</th>
		<th width="13%">Conformance</th>
		<th width="13%">Associated Coded Profiles</th>
	</tr>
	<tr>
		<td>
			<a href="explore_allergies_and_adverse_reactions.html">Allergies and adverse reactions</a>
		</td>
		<td>886921000000105</td>
		<td>0..1</td>
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
		<td>0</td>
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
		<td>1..1</td>
		<td>Mandatory</td>
		<td>2</td>
	</tr>
	<tr>
		<td>
			<a href="explore_discharge_details.html">Discharge details</a>
		</td>
		<td>886811000000106</td>
		<td>0..1</td>
		<td>Required</td>
		<td>1</td>
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
			<a href="explore_information_and_advice_given.html">Information and advice given</a>
		</td>
		<td>1052951000000105</td>
		<td>1..1</td>
		<td>Mandatory</td>
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
			<a href="explore_referrer_details.html">Referrer details</a>
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
</table>


## Overview of Emergency Care eDischarge Sections and Coded profiles ##
This diagram illustrates the sections used in Emergency Care eDischarge and which sections allow coded representation of the section text. 


<a href="images/explore/EC_composition_overview.png" target="_blank" style="width: 100%;max-width: 100%;"><b>Click to open in new window</b></a>


<img src="images/explore/EC_composition_overview.png" style="width:auto;height: auto;"/>



The text sections are carried in the FHIR Composition Resource. 
This is profiled as the [CareConnect-ITK-EC-Compostion](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-EC-Composition-1)





