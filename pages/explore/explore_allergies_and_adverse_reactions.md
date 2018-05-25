---
title: Allergies and Adverse Reactions Section
keywords:  messaging, sections
tags: [fhir,messaging,section]
sidebar: foundations_sidebar
permalink: explore_allergies_and_adverse_reactions.html
summary: "Gives information about the Allergies and adverse reactions section"
---

{% include custom/section.warnbanner.html %}

## Allergies and Adverse Reactions Section Content##
The Allergies and adverse reactions section carries information about the patient's allergies and adverse reactions. Elements should be formatted as subheadings in any HTML sent.
Where a value is marked as Text derived from SNOMED CT the section on [constructing clinical coded structures](build_allergy_lists.html) should be consulted for further information. 

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
   <td>Allergies and adverse reactions</td>
   <td>The details of any known allergies, intolerances or adverse reactions.</td>
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
   <td>Causative agent</td>
   <td>The agent such as food, drug or substances that has caused or may cause an allergy, intolerance or adverse reaction in this patient. Or "No known drug allergies or adverse reactions" Or "Information not available"</td>
   <td>1 only</td>
   <td>mandatory</td>
   <td>Choice of Text or Text derived from SNOMED CT  -  constraint: SNOMED CT: Allergy Archetypes Drug Groups. NHS dm+d TF,NHS dm+d TFG,NHS dm+d VMP,NHS dm+d AMP,NHS dm+d Ingredients,NHS dm+d Combination drug VTMs,</td>
  </tr>
  <tr>
   <th>Reaction details cluster</th>
   <th>&nbsp;</th>
   <th>&nbsp;</th>
   <th>&nbsp;</th>
   <th>&nbsp;</th>
  </tr>
  <tr>
   <td>Description of reaction</td>
   <td>A description of the manifestation of the allergic or adverse reaction experienced by the patient. For example, skin rash.</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Choice of Text or derived from SNOMED CT - constraint: SNOMED CT. Clinical finding. Any SNOMED CT term in the Clinical Finding hierarchy. Constraint binding: [SNOMED CT] subset=Clinical Finding</td>
  </tr>
  <tr>
   <td>Severity</td>
   <td>A description of the severity of the reaction</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Text derived from SNOMED CT - Mild [The reaction was mild.][SNOMED-CT::255604002] (Mild (qualifier value))•  Moderate [The reaction was moderate.][SNOMED-CT::6736007] (Moderate (severity modifier) (qualifier value))•  Severe [The reaction was severe.][SNOMED-CT::24484000] (Severe (severity modifier) (qualifier value))•  Life threatening [The reaction was life-threatening.][SNOMED-CT::442452003] (Life threatening severity (qualifier value))•  Fatal [The reaction was fatal.][SNOMED-CT::399166001] (Fatal (qualifier value))</td>
  </tr>
  <tr>
   <td>Certainty</td>
   <td>A description of the certainty that the stated causative agent caused the allergic or adverse reaction.</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Text derived from SNOMED CT - Unlikely [The reaction is thought unlikely to have been caused by the agent.][SNOMED-CT::1491118016]•  Likely [The reaction is thought likely to have been caused by the agent.][SNOMED-CT::5961011]•  Certain [The agent is thought to be certain to have caused the reaction but this has not been confirmed by challenge testing.][SNOMED-CT::255545003] (Definite (qualifier value))•  Confirmed by challenge testing [The reaction to the agent has been confirmed by challenge testing or other concrete evidence.][SNOMED-CT::410605003] (Confirmed present (qualifier value))</td>
  </tr>
  <tr>
   <td>Comment</td>
   <td>Any additional comment or clarification about the adverse reaction.</td>
   <td>0 to 1</td>
   <td>required</td>
   <td>Free text</td>
  </tr>
 </tbody>
</table>

## How to Represent "No Know Allergies" ## 
When there is a positive statement that the patient has "No know allergies" then no coded structure is sent and the section is sent with a text string within the narrative. When the text string is derived from coded data it must match the text of the code: for example 716186003 "No Known allergy"

##  Example Allergies and Adverse Reactions Sections ##

### Allergy to Penicillin ###

<script src="https://gist.github.com/IOPS-DEV/c02f9626ad71d2230cd51ded6d031bb2.js"></script>

### "No known Allergy" ###

<script src="https://gist.github.com/IOPS-DEV/3f77d2ebcfcdf305a640484fb445cc1a.js"></script>

## Coded Resources ##

This text section should be linked to the following FHIR Resources to provide the textual information in a coded format.

- List
- AllergyIntolerance
- Flag
 
See constructing coded clinical structures - [Allergy Lists](build_allergy_lists.html)











