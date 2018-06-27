---
title: Safeguarding Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_safeguarding.html
summary: "Gives information about the Safeguarding section"
---

{% include custom/section.warnbanner.html %}

## Safeguarding Section Content ##
The Safeguarding section carries details of any safeguarding concerns. Elements should be formatted as subheadings in any HTML sent.


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
   <td>Safeguarding</td>
   <td>Details of any identified safeguarding concerns.</td>
   <td>&nbsp;</td>
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
   <td>Safeguarding issue</td>
   <td>A record of any identification of concerns regarding safeguarding during attendance</td>
   <td>0 to many</td>
   <td>R</td>
   <td>Text only and if applicable the text should reflect the values in the ECDS SNOMED CT Safeguarding subset.</td>
  </tr>
  <tr>
   <td>Comment</td>
   <td>A comment providing further detail on a safeguarding issue.</td>
   <td>0 to 1</td>
   <td>R</td>
   <td>Free text</td>
  </tr>
		<tr>
		<td colspan="5"><b>* M=Mandatory R=Required O=Optional</b></td>
		</tr>
 </tbody>
</table>

##  Example Safeguarding Section ##

<script src="https://gist.github.com/IOPS-DEV/11ae32acda7827d537f2aa6e56327f5e.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK3 FHIR Emergency Care eDischarge does not currently support a coded safeguarding.


