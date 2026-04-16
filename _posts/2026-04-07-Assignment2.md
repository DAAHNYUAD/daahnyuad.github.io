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

## DRAFT Guidelines for the Assignment:  

The Mapping Assignment, otherwise known as Assignment 2, will be completed in one step. It builds on work we did in the textual portion of the class, particularly with attempting to annotate "Souther Arabia" by Mr and Mrs Theodore Bent and to automatically geocode "1, the Road" by Ross Goodwin. This assignment can be done *alone* or *in pairs*.


- **Format**: Individual or pairs (maximum 2 people)
- **Length**: Approximately 1500 words (about an 8-minute read), plus visuals
- **Due Date**: Saturday, 26 April 2026. 


This exercise has three main elements: 

1. **Manual Annotation with Recogito**: You will be provided with a text to annotate manually in Recogito. 
2. **Supplementary Annotation**: using other digital means--Google Maps, OSM, etc., you will complete to whatever extent is possible your geo-annotation.
3. **Comparison with Automated Geocoding**: You will be provided with a Assemble your evidence, analysis, and visuals in a web-published essay in the form of a post that tells a coherent story about your findings. Make sure that one of your Voyant Tools visualization is a live widget embedded in your post. 

## **Step 1**: The Text and its Author

The text you will annotate in Recogito contains more of the text of "Southern Arabia" by Theodore and Mabel Bent (Project Gutenberg text #21569). This is the same text for which we annotated the section about the Yemeni island of Socotra. The passage in question will be the first half of the travel through the Hadr al Mot (the Hadhramout).

## **Step 2**: Research the Text in Question

Before you begin analysis, research the texts themselves: Who are the authors? What is the publication context? What are the general themes and contents? You can learn more about its authors [here](https://en.wikipedia.org/wiki/James_Theodore_Bent). Feel free to use anything you learned in the homework assignment about Socotra. 

> The more you know about the text, the more meaningful your analysis will be. 

## **Step 3**: Annotating in Recogito
Upload the provided txt file into your own account in Recogito by clicking on the blue `add` button. If you are working on this in a pair, one of you can add the file, and then share it with the other. Do this by opening the file and then from document settings, click on `sharing` and adding the user name of your partner. 

Before you begin annotating, in `annotation preferences` unclick all of the gazetteers, except HistoGIS, Pleiades and GeoNames. 

Navigate to `document view` and annotate as much as you can from it. If you do not find place names in the gazetteers mentioned above, you can use other sources (Wikipedia, Google Maps, etc) and insert latlongs into the comment field. 

When you are done with your annotation, fill out the metadata in `document settings` and opt for the "out of copyright in territory of publication" license and save. Then in the `sharing` tab at left set public access to "anyone with the link" and include the link to the document in your write up.   

## **Step 4**: Downloading and Cleaning 

Using "download options" download a csv version of your dataset and do any cleaning necessary. In particular, you may need to move any geodata from the comments field to the latlong fields. 

Once you have downloaded the data and gotten the link from Step 3, you are done with Recogito. 

## **Step 5**: Visualizing the Data

You will have two datasets to visualize in this step. The first one has been automatically generated from the excerpt mentioned above. I have used a similar script for geographical entity recognition that I used to do that for the "I, the Road" exercise. That file can be found [here](). 

The script works with the leaflet package in R to create an html map with two layers. It also performs a very slight distortion of the points on the map to prevent overlap (occultation) to make the next step easier.

Once you have saved an html file to your satisfaction using the notebook, download it out of posit.cloud. 

The last step of visualization is to push it to your Github page. 

## **Step 6**: Conduct your Analysis 

In this last step of the exercise, you can compare the visual results and the structured data on which they depend in order to compare the processes of manual and automatic geocoding to what kinds of differ in human and machine approaches.


## Guiding Questions (you do not need to answer all these questions):

- **Background & Expectations**: 

- **Computational Insights**: 

- **Comparative Insights**: 

- **Trends & Surprises**: 

- **Methodological Questions**: 

- **Scope & Scale**: 

- **Transferability**: 


## Assessment

Your work will be assessed according to the following criteria located [here](https://djwrisley.github.io/RLAC/rubrics/).

## Tips for Success

**Writing**: Use tools like [Markdown Live Preview](https://markdownlivepreview.com/) and [Hemingway App](https://hemingwayapp.com/) to refine your prose for clarity and legibility, without AI. Keep the [F-shape principle](https://www.nngroup.com/articles/f-shaped-pattern-reading-web-content/) for web writing in mind—readers scan top-to-bottom and left-to-right, so structure your argument visibly.

**Visualization**: Make your screenshots speak. Use clear captions that explain what readers are seeing and why it matters to your argument. Your visualizations should support and enhance your analysis, not merely decorate it or fill space. Feel free to annotate on top of the visuals (like putting arrows or circles).

**Collaboration**: If working in pairs, you may submit a single essay that links to both group members’ sites. Include a brief statement describing each person’s unique contribution to the work.

**Publishing**: Post your assignment to your course site as a post so instructors and classmates can read and engage with your work.

It is fine to publish your assignment iteratively, but when you finish the final version of your assignment, write at the bottom of it “READY FOR GRADING”.

Good luck with your analysis!