---
title: "Assignment 3 Visual AI and Culture S25"
excerpt_separator: "<!--more-->"
categories:
  - Blog
tags:
  - Assignments
  - Corpora
  - F25
  - distant viewing
  - images
---


## Final Guidelines for the Assignment:  

In this assignment we will continue to work with materials and algorithms discussed in class to explore a custom-made corpus of digital images. We will use Orange Data Mining, 2DCLIP and DV Explorer to explore this corpus and then write a small critical essay based on our findings. This can be worked on in pairs, or alone. 

### Part One: 

The very first thing you have to do is to build an image dataset, a corpus. You should choose a corpus of images, made up of at least 75 images.  

## Guidelines for the Corpus building exercise: 

- a dataset of images from a cultural domain is required, one about which you know a little *or a lot* is welcome. 
- it does not have to be "high" cultural or from the GLAM sector. 
- it does not have to be designed with computation in mind.
- it should address something that you suspect is not close to Microsoft COCO or Google's Inception training. 
- its collection can be automated, but does not have to be.
- it should not have faces of people in them.  

## Tips on automating the collection: 

You could think about automating this process by using certain extensions such as Image Downloader, or by learning how to scrape images. Remember that part of building a corpus will be the organization of those images into categories, and potentially the renaming of them. You will want to keep track of where you get them and cite that as part of your corpus building exercise. 

You may end up collecting some of the images and then removing or adding others later, particularly in the move between part two and parts three and four. 


### Part Two: 

The first computational exercise is a clustering exercise. Some prior knowledge of the subject is important since in the second part you will classify the images into subtypes. Choosing a dataset of images you are not very interested in, or a dataset that you do not have enough knowledge to categorize will make it difficult.  

I suggest you use this part of the assignment to do some exploratory data analysis (EDA). Using the pre-set Orange Data Mining workflow I distributed (images2.ows), you can address the following questions: 

- How does one built-in algorithm such as Inceptionv3 in ODM cluster the data? 
- Do other algorithms give you different results? 
- What features seem to be most characteristic of the different quadrants of the image plot? 
- Using hierarchical clustering, isolate specific clusters to look more closely.
- How "in reading a corpus of visual culture through a neural network, [are you] always also doing the reverse?" (Impett and Offert, 2024)

Make screenshots of the main image plot you generate and annotate it with labels (just typed on manually with a program like Preview) which illustrate in your opinion what combination of features are represented in each of the four quadrants of the plot. Caption the image with the relevant information (i.e. Image Plot generated with Orange Data Mining and the algorithm of your choice). Also include image plot of specific clusters that can help you to understand how the out-of-the-box algorithms (think of the [Monet/Manet video](https://orangedatamining.com/blog/clustering-of-monet-and-manet/)).

Be sure to comment on how differently you see the images. 

### Part Three:

In the second computational exercise you will categorize the images using Orange Data Mining into at least two different groupings, although more than 2 are suggested. The categorization is carried out by placing the images into subfolders (each bearing a descriptive title). This means that for the purposes of your assignment, you should have two or three copies of the same images, but organized in different folders according to categories you have chosen (e.g. size, shape, color OR origin, quantity, size). For best results, your classification system should be sure to have a somewhat equal number of images in every category. 

For each of the sets of images, please generate a confusion matrix and assess the ability of the chosen algorithm (Inception, VGG, OpenFace, etc) to predict the categories you have chosen. Remember that you can click on the box where there has been misclassification and visualize the misclassified objects in the viewer. Discussing what the model got wrong, can be very interesting (perhaps more interesting than what it got right).

Guiding questions for this part of the assignment: 

- How well did any of the built-in algorithms you chose predict the categories you established?
- Did you go back and adjust any of your categories and retry. What was the rationale for adjusting your categories
- When you isolate the cases of "false positives", i.e. mis-predictions, can you understand why the algorithm got them wrong? (Think about the Monet/Manet mis-prediction case we saw in class).
- If you could train your own algorithm to look at specific features or deal with specific kinds of data, what would you aim to teach it? 

In your write up, you should include insights and ideas from the new book Distant Viewing (Arnold & Tilton), linked to on the syllabus. 

Make sure that you include images from your analysis. 

### Part Four:

In the third computational exercise, I want you to work with multimodal models and your image corpus. 

The first way that you can explore a multimodal model is to use the 2DCLIP tool created by my colleague. It only works on specific browsers, so pay attention to that. When you upload the images to the tool, you get to choose the x and y axis descriptions. Try a variety of these and comment on how it works. As we saw in class, it does not work necessarily well if you pick opposites (hot and cold, high and low culture, etc.) Nonetheless, the choice of keywords or expressions does affect the clustering that you get. 

Here I suspect the insight from Impett & Offert ("in reading a corpus of visual culture through a neural network, we are always also doing the reverse") will be very obvious. 

The second way that you can explore a multimodal model is to use DV Explorer. In particular you can use two tools there, [5.1 Zero-Shot](https://distantviewing.org/dvexplorer/pages/zeroshot/) and/or [5.2 Image Caption](https://distantviewing.org/dvexplorer/pages/caption/). In the first one that "extends and combines the ideas behind object detection and image embedding" you can upload a set of images and then create a similarity score for a given textual description. Instead of seeing the images in an image grid (as in 2D CLIP) you get them in order of similarity. In the second, you give DV Explorer an image and a textual caption is created. You could do this for a selection of images and compare the captions with the cultural specificity of the images you have or with the object detection suggestions. 

NB: You do not have to engage with all of these multimodal explorations, but do at least one. 

Guiding questions for this part of the assignment:

- how well does the process work for the pre-computed embeddings for the included image sets work compared to your custom set of images? 

- The algorithm for 2DCLIP and Zero-Shot models is different. Do you get very different results from either of them for the same images or keywords? 

- what kinds of culturally or historically specific features are not captured by the models?

- to what extent is this exercise a kind of reading of the neural network? 

## What to include in your assignment

Since this is a visual assignment, you are not limited in the number of images you can use. As in previous assignments, screenshots of key points that match your analysis will be graded the highest. If you depart from the exercise at all and use code, or other means for acquiring or manipulating the image data, please explain and include that code (if appropriate). If you feel comfortable sharing the images in GitHub you can do so in the assets folder. If not, make sure that you make the images available for me to look at in Drive with a link shared for me. Be sure to connect your writing with any links to resources that are important for your reader. Also, connect your analysis to anything from the book _Distant Reading_ or the other articles from the third section of class. 



Due Date for this assignment: 11 May 2025, noon, 1500 words maximum. 
