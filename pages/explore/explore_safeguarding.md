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
The Safeguarding section carries details of any safeguarding concerns. Elements should be formatted as subheadings in any html sent:

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
   <td>Safeguarding</td>
   <td>Details of any identified safeguarding concerns.</td>
   <td>&nbsp;</td>
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
   <td>Safeguarding issue</td>
   <td>A record of any identification of concerns regarding safeguarding during attendance</td>
   <td>0 to many</td>
   <td>required</td>
   <td>ECDS SNOMED CT Safeguarding subset.Text.</td>
  </tr>
  <tr>
   <td>Comment</td>
   <td>A comment providing further detail on a safeguarding issue.</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Free text</td>
  </tr>
 </tbody>
</table>

##  Example Safeguarding Section ##

<script src="https://gist.github.com/IOPS-DEV/598b9ff335715b03d0264a03f2442d34.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK FHIR Emergency Care eDischarge does not currently support a coded safeguarding.


