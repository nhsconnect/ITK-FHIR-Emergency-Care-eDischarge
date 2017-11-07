---
title: Richard Smith Emergency Care Scenario
keywords: workflow
tags: [development,fhir,profiles]
sidebar: overview_sidebar
permalink: engage_richard_smith.html
summary: "Example scenario - Richard Smith Emergency Care"
---

{% include custom/search.warnbanner.html %}

## Background ##

Richard Smith aged 60, is at home and has been feeling unwell with chest pain. His wife speaks to Peter, a neighbour, who offers to take them to the local A & E department. On arrival at A & E, with the aid of his wife Richard checks in with the receptionist. 

The receptionist asks for his name, address and date of birth and does a PDS look-up to get his details. She confirms these are correct and checks Richard in on the A & E system. She then asks him to take a seat in the waiting area.

## The A & E Department Encounter ##

The A & E Department encounter is carried in the [Encounter Resource](https://fhir.nhs.uk/STU3/StructureDefinition/CareConnect-ITK-Encounter-1)

**Named Participants**

- Patient - **Richard Smith** - [Patient Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Patient-1)
- Patient's wife - **Joy Smith** - [RelatedPerson Resource](https://fhir.nhs.uk/STU3/StructureDefinition/ITK-RelatedPerson-1)
- Consultant - **Mr Abacus** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Discharging clinician (Document Author) - **Dr Paul Rastall** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Patient's GP (Document recipient) - **Dr John Lorenzo** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)
- Community Nurse (Document recipient) - **Mrs Angela Jones** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)

**Named Organisations**

- Patient's GP Practice - **MGP Medical Centre** - [Organization Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Organization-1)
- Discharging Hospital - **Leeds Teaching Hospitals NHS Trust** - [Practitioner Resource](https://fhir.hl7.org.uk/STU3/StructureDefinition/CareConnect-Practitioner-1)


After a short wait, Richard starts to feel worse and his wife goes to speak to the receptionist, who asks a passing nurse to speak to Richard. Richard's wife explains that she is concerned about the possibility of Richard suffering from a heart attack,as his symptoms are similar to Richard's mother when she had a heart attack. The nurse feels that Richard needs to be seen urgently and asks him and his wife to follow her to the examination cubicle. After taking Richard's vital signs, the nurse explains that she will go and get a doctor to examine Richard. She leaves the cubicle and returns with Dr Paul Rastall. He also takes Richard's vital signs and does an ECG that shows inferior ischaemic changes. Dr Paul Rastall explains that he may need to admit Richard but will speak to the consultant Mr Abacas, who after reviewing the ECG agrees that Richard should be admitted a ward for further tests without delay. 

Dr Paul Rastall updates the A & E system and sends an Emergency Care eDischarge to Richard's GP and the community nurse. The Emergency Care eDischarge give a summary of the A & E encounter and informs the GP that Richard has been admitted to a ward for further tests. 

## Example Instance of Scenario ##

<script src="https://gist.github.com/IOPS-DEV/1a532eb43b226dcd6ce26a6b698019f4.js"></script>

## Example Rendered Instance of Scenario ##