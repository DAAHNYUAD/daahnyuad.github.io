---
title: "Assignment 3 Visual AI and Culture F26"
excerpt_separator: "<!--more-->"
categories:
  - Blog
tags:
  - Assignments
  - Corpora
  - F26
  - distant viewing
  - DVExplorer
  - Orange Data Mining
  - images
---


## Guidelines for the Assignment:  DRAFT

In this assignment we will continue to work with materials and algorithms discussed in class since 5 November to explore a custom-made corpus of digital images. We will use DV Explorer and Orange Data Mining to explore this corpus and then write a small critical essay based on our findings. This can be worked on in pairs, or alone. It has four or five parts. 

### Part One: 

The very first thing you have to do is to build an image dataset, a corpus. You should choose a corpus of images, made up of at least 150 images. 

## Guidelines for the Corpus building exercise: 

- a dataset of images from a cultural domain is required, one about which you know a little *or a lot* is welcome. 
- it does not have to be "high" cultural or from the GLAM (Galleries, Libraries, Archives and Museums) sector. I do not want you to take a pre-made dataset from another site, say Kaggle or the like.
- it does not have to be designed with computation in mind.
- it should address something that you suspect is not close to Microsoft COCO or Google's Inception training. 
- its collection can be automated (with Image Downloader, for example), but it does not have to be.
- it can come from multiple accounts, sites, or a search engine, but the process of collection should be explained.
- it should perferably not have faces of people who are alive in them.  

## Tips on automating the collection: 

You could think about automating this process by using certain extensions such as Image Downloader for Chrome, or by learning how to scrape images. Remember that part of building a corpus will be the organization of those images into categories, and potentially the renaming of them. You will want to keep track of where you get them and explain that as part of your corpus building exercise. 

Some prior knowledge of the subject is important since in the second part you will classify the images into subtypes. Choosing a dataset of images you are not very interested in, or a dataset that you do not have enough knowledge to categorize will make it difficult.  

You may end up collecting some of the images and then removing or adding others later, particularly in the move between part two and parts three and four. 

### Part Two: 

The first computational exercise is a clustering exercise, of the "let-the-data-group-itself" sort. 

I suggest you use this part of the assignment to do some exploratory data analysis (EDA). Using the pre-set Orange Data Mining workflow I distributed (images.ows), you can address the following questions: 

- How does one built-in algorithm such as Inceptionv3 in Orange Data Mining cluster the data? Do other algorithms give you different results? Try at least two. 

Here is how Gemini compares the various models: 

| Model | Vector Size | Model Size | Speed | Main Strength | Best Use Case |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **InceptionV3** | **2,048** | ~92 MB | Fast | Captures multi-scale details accurately | General image search & clustering |
| **VGG16** | **4,096** *(or 512 pooled)* | ~528 MB | Slow | Preserves fine textures & visual styles | Style transfer & texture matching |
| **VGG19** | **4,096** *(or 512 pooled)* | ~549 MB | Slowest | Slightly deeper version of VGG16 | Legacy baselines (usually skip) |
| **SqueezeNet** | **1,000** *(or 512 pooled)* | **less than 5 MB** | **Fastest** | Ultra-lightweight with tiny memory footprint | Mobile apps, edge devices, & CPU-only runs |

- What features seem to be most characteristic of the different quadrants of the image plot? 
- Using hierarchical clustering, isolate specific clusters to look more closely. What are the groups that it suggests? Do these correspond to the way that you would group them? 
- Pick a group that is not so clear to you and propose a few possibilities.
- How "in reading a corpus of visual culture through a neural network, [are you] always also doing the reverse?" ([Impett and Offert, 2023](https://arxiv.org/abs/2308.07464))

Make screenshots of the main image plot you generate and annotate it with labels (just typed on manually with a program like Preview) which illustrate in your opinion what combination of features are represented in each of the four quadrants of the plot. Caption the image with the relevant information (i.e. Image Plot generated with Orange Data Mining and the algorithm of your choice). Also include image plot of specific clusters that can help you to understand how the out-of-the-box algorithms (think of the [Monet/Manet video](https://orangedatamining.com/blog/clustering-of-monet-and-manet/)).

Be sure to comment on how differently you see the images. 

### Part Three:

In the second computational exercise you will categorize the images using Orange Data Mining into four or more different groupings. The categorization is carried out by placing the images into subfolders (each bearing a descriptive title). This means that for the purposes of your assignment, you should make a copy of the same images, but organized in different folders according to categories you have chosen (e.g. content, style, shape, color, complexity, creator). For best results, your classification system should be sure to have a **somewhat equal number of images** in every category. 

> For part three, you might have to tweak your original dataset from part two so that you have the balance and categories necessary for the exercise.  

For each of the sets of images, please generate a confusion matrix and assess the ability of the chosen algorithm (Inception, VGG, OpenFace, etc) to predict the categories you have chosen. Remember that you can click on the box where there has been misclassification and visualize the misclassified objects in the viewer. 

### Part Four (optional): DV Explorer 

You may want to return to DV Explorer to try out some of its features with the uncategorized version of the dataset (from Part Two) to see if they inform the observations you made above.

### Part Five: Discussion

Discussing what the model got wrong, can be very interesting (perhaps more interesting than what it got right). You may discuss parts 2 and 3 together or separately. 

Guiding questions for the discussion part of the assignment: 

- How well did any of the built-in algorithms you chose predict the categories you established?
- Did you go back and adjust any of your categories and retry. What was the rationale for adjusting your categories?
- When you isolate the cases of "false positives", i.e. mis-predictions, can you understand why the algorithm got them wrong? (Think about the Monet/Manet mis-prediction case we saw in class).
- If you could train your own algorithm to look at specific features or deal with specific kinds of data, what would you aim to teach it? 

In your write up, you should include insights and ideas from the book Distant Viewing (Arnold & Tilton) on the importance of labeling, [ch 1](https://direct.mit.edu/books/oa-monograph/5674/chapter/4361339/Distant-Viewing-Theory). 


## What to include in your assignment

Since this is a visual assignment, you are not limited in the number of images you can use. As in previous assignments, screenshots of key points that match your analysis will be graded the highest. If you depart from the exercise at all and use code, or other means for acquiring or manipulating the image data, please explain and include that code (if appropriate). If you feel comfortable sharing the images in GitHub you can do so in the assets folder. If not, make sure that you make the images available for me to look at in Drive with a link shared for me. Be sure to connect your writing with any links to resources that are important for your reader. Also, connect your analysis to anything from the book _Distant Reading_ or the other articles from the third section of class. 



Due Date for this assignment: 14 December 2026, 1159pm, 1500-2000 words maximum. 
