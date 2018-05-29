---
title: Plan and requested actions Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_plan_req_actions.html
summary: "Gives information about the Plan and requested actions section"
---

{% include custom/section.warnbanner.html %}

## Plan and Requested Actions Content ##
The Plan and requested actions section carries information about planned and requested actions such as planned investigations, procedures etc. Elements should be formatted as subheadings in any HTML sent.

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
   <td>Plan and requested actions</td>
   <td>The details of planned investigations, procedures and treatment, and whether this plan has been agreed with the patient or their legitimate representative.</td>
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
   <td>Action</td>
   <td>Including planned investigations, procedures, Interventions and treatment for a patient's identified conditions and priorities. For each action the following should be identified:
<ul>
<li>a) person responsible - name and designation / department / hospital / patient etc or role (eg GP) responsible for carrying out the proposed action, and where action should take place.</li>
<li>b) status - requested, planned or completed.</li>
<li>c) When action requested for - requested date, time, or period - as relevant.</li>
<li>d) suggested strategies - suggested strategies for potential problems.</li>
<li>e) outcome expectations, including patient's expectations</li></ul></td>
   <td>1 to many</td>
   <td>mandatory</td>
   <td>A record of the planned and requested actions. May be structured (table), with actions, names, dates, status, location, strategies, or free text</td>
  </tr>
 </tbody>
</table>

##  Example Plan and Requested Actions Section ##

<script src="https://gist.github.com/IOPS-DEV/1cfc7a85e79b3f9cfaf260c7d8c2f24e.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- The ITK3 FHIR Emergency Care eDischarge does not currently support coded Plan and requested actions information.






