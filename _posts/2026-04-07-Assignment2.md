---
title: "Assignment 2 Manual Geocoding vs Automated Geocoding S26"
excerpt_separator: "<!--more-->"
tags:
  - Assignments
  - Corpora
  - S26
  - R
  - Markdown
  - Recogito
---

## FINAL Guidelines for the Assignment:  

The Mapping Assignment, otherwise known as Assignment 2, will be completed in one step. It builds on work we did in the textual portion of the class, particularly with attempting to annotate _Southern Arabia_ by Theodore and Mabel Bent and to automatically geocode "1, the Road" by Ross Goodwin. 

> Manual geocoding is essentially human interpretation of places and matching them with possible geographic places using contextual clues. Automatic geocoding is based on a machine identifying possible place names and matching those against databases without contextualization. 

## About the Text

The text you will annotate in Recogito contains more of the text of _Southern Arabia_ by Theodore and Mabel Bent (Project Gutenberg text #21569). This is the same text for which we annotated the section about the Yemeni island of Socotra. The passage in question will be the first half of the travel through the Hadr al Mot (the Hadhramout).

_Southern Arabia_ reflects a late 19th-century imperial gaze that portrays South Arabian societies in an exotic light, making reference to a number of Western-centric cultural references. The text is found in Project Gutenberg as a digital text, but the authors' perspectives raise questions about the representativeness of its ethnographic and historical claims. Despite its biases, the text provides a rich example for testing spatial tagging while critically examining how computational tools surface—and sometimes reproduce—colonial viewpoints.

The portion of the text you will use is located [here](https://raw.githubusercontent.com/DAAHNYUAD/daahnyuad.github.io/refs/heads/master/assets/texts/Bents_Hadhramout.txt).

## Assignment Details

- **Format**: Individual or pairs (maximum 2 people)
- **Length**: Approximately 1500 words (about an 8-minute read), plus visuals
- **Due Date**: Saturday, 26 April 2026. 
- This assignment can be done *alone* or *in pairs*.

This assignment has three main elements: 

1. **Manual Annotation with Recogito**: You will be provided with a text to annotate manually in Recogito. 
2. **Supplementary Annotation**: using other digital means--Google Maps, OSM, etc., you will complete to whatever extent is possible your geo-annotation.
3. **Comparison with Automated Geocoding**: You will be provided with the automatically tagged text and structured geodata for this section. Assemble your evidence, analysis, and visuals in a web-published essay in the form of a post that tells a coherent story about your findings. 

## **Step 1**: Research the Text in Question

Before you begin analysis, research the texts themselves: Who are the authors? What is the publication context? What are the general themes and contents? You can learn more about its authors [here](https://en.wikipedia.org/wiki/James_Theodore_Bent). Feel free to use anything you learned in the homework assignment about Socotra. 

## **Step 2**: Annotating in Recogito

Upload the provided txt file in `/assets/texts` into your own account in Recogito by clicking on the blue `add` button. If you are working on this in a pair, one of you can add the file, and then share it with the other. Do this by opening the file and then from document settings, click on `sharing` and adding the username of your partner. 

Before you begin annotating, in `annotation preferences` unclick all of the gazetteers, except HistoGIS, Pleiades and GeoNames. 

Navigate to `document view` and annotate as much as you can from it. If you do not find place names in the gazetteers mentioned above, you can use other sources (Wikipedia, Google Maps, etc) and insert latlongs into the comment field. 

When you are done with your annotation, fill out the metadata in `document settings` and opt for the "out of copyright in territory of publication" license and save. Then in the `sharing` tab at left set public access to "anyone with the link" and include the link to the document in your write up.   

## **Step 3**: Downloading and Cleaning 

Using `download options` download a csv version of your dataset and do any cleaning necessary. In particular, you may need to move any geodata from the comments field to the latlong fields. 

Once you have downloaded the data and gotten the link from Step 3, you are done with Recogito. 

## **Step 4**: Visualizing the Data

You will have two datasets to visualize in this step. The first one has been automatically generated from the excerpt mentioned above. I have used a similar script for geographical entity recognition using a library called `spaCy` and geocoding with `geopy` that I used to do that for the "I, the Road" exercise. That file can be found [here](https://raw.githubusercontent.com/DAAHNYUAD/daahnyuad.github.io/refs/heads/master/assets/datasets/Bents_Hadhramout_places_geocoded.csv) in \assets\datasets. 

For step 4, you should use the notebook in posit.cloud entitled "". The notebook employ the `leaflet` package in R to create an html map with two layers. It also performs a very slight distortion of the points on the map to prevent overlap (occultation) to make the next step easier.

Once you have saved an html file to your satisfaction using the notebook, download it out of posit.cloud. 

The last step of visualization is to push it to your Github page. ...

## **Step 6**: Conduct your Analysis 

In this last step of the exercise, you can compare the visual results and the structured data on which they depend in order to compare the processes of manual and automatic geocoding to what kinds of differ in human and machine approaches.


## Guiding Questions (you do not need to answer all these questions):

**Observations**: 
- Do you observe any patterns when comparing the manually and automatically geocoded locations?
- Do the two methods produce similar coordinates or mappings?
- Where do the largest discrepancies occur (distance, region, or level of precision)?

**Agreement/disagreement of the two methods**:
- Identify one or two cases where manual and automatic geocoding differ significantly. What is happening in those examples?
- Are mismatches random, or do they follow patterns (e.g., ambiguous place names, incomplete data)?
- Are certain types of locations (cities, regions, historical places) more prone to disagreement? 

**Data and Sensitivity**: 
- How does the quality or completeness of the original place names affect each method? Do you remember what happened when we added on the state name for the locations in "1, the Road"? 
- What happens when place names are: misspelled, come from a different language, are historical or vague (e.g., “near Cairo”).

**Interpretation vs automation**: 
- What kinds of decisions are humans making in manual geocoding that automated systems cannot easily replicate?
- What assumptions does the automated system make when matching place names to coordinates?
- How does each method handle ambiguity (e.g., multiple places with the same name)?

**Critical Questions**: 
- What kinds of places or regions might be systematically misrepresented by automated geocoding systems?
- How might linguistic, historical, or cultural variation affect geocoding accuracy?
- What does this comparison reveal about the limits of computational approaches to spatial data?

## Assessment

Your work will be assessed according to the following criteria located [here](https://djwrisley.github.io/RLAC/rubrics/).

## Marking your work as complete

It is fine to publish your assignment iteratively, but when you finish the final version of your assignment, write at the bottom of it “READY FOR GRADING”.

Good luck with your analysis!