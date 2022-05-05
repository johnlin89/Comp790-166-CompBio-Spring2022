# Comp790-166: Computational Biology (Spring 2022) 

## Details

Instructor: Natalie Stanley

Email: natalies@cs.unc.edu

**Note : Please send me an email if you enrolled late and did not recieve the welcome email!**

Time and Place: Monday/Wednesday 9:30am-10:45am in Sitterson 115 (SN0115) and on Zoom. This course will be offered as a hybrid course. I will be present in SN0115 for each class meeting and also be on zoom and recording the lecture. Please watch your emails for a zoom link. 

 Info and Attributes: This is a 3-credit full-semester course and fulfills the 'Applications' category for CS students. It is a lecture-style class (I will teach the lectures) and includes two homework assignments and a course project. Please make sure you selected the 3-credit option when you enrolled. 

Office Hours: Monday 10:45-noon or by appointment 

## Description
Modern, high-throughput assays allow us to efficiently profile a variety of biological processes to gain a systems-level understanding of health and disease. Recent technologies and experimental assays generate an abundance of detailed information that needs to be extracted, summarized, and interpreted. In this course we will discuss the methodology used to extract signal from (e.g. process, engineer features from, combine, etc.) data generated by some of the most cutting-edge experimental paradigms, such as single-cell assays and imaging. We will go into detail about the methods and theory underlying bioinformatics algorithms, originating from numerical linear algebra, graph-signal processing, and machine learning. While computational biology is a very broad field, we will focus here on applications in single-cell biology (CyTOF, single-cell RNA sequencing), multiomics/multi-modal analysis, systems immunology, and benchmarking. For each class of algorithms introduced for some task on biological data, we will also go over necessary theory and mathematical intuition. The course covers the foundations for biomedical data science and does not assume any biological knowledge.

## Prerequistes
Students should be strong in programming in Python or Julia or R, and be comfortable with linear algebra and basic probability. **I do not assume any prior biological knowledge. Any relevant concepts will be introduced**. Please feel free to talk to me about any of these prerequistes. 

## Course Structure
This course will be mostly lecture-based with two homework assignments and a course project. I will provide ideas for several publicly available biological datasets and open problems for you to work on for these projects. Overall, the project is intended to give you an opportunity to implement/apply methodology discussed in the papers that we will discuss together. The final project writeup will also give you practice writing up results and communicating ideas. You are welcome to work on teams for this project.

Students will also pick any two days during the semester to answer a set of reading questions about one of the assigned papers. 

# Topics and Tentative Schedule. 

This is the preliminary set of topics. 


| Date | Topic | Reading | Notes | Code |
|------|-------|---------|-------|------|
|Monday January 10, 2022 | Intro, Bioinformatics vs Computational Biology| [[Systems Immunology, Just Getting Started](https://www.nature.com/articles/ni.3768)], [[Grand Challenges in Single-Cell Data Science](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-020-1926-6)] | [[Lecture 1 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture1_public.pdf)] | 
|Wednesday January 12, 2022| Linear Algebra Review, Matrix Rank, Building Graphs from Data, Graph Laplacian, Graph Diffusion | [[SLMP. pages 10-22](https://arxiv.org/abs/2004.07984)], [[Data Matrices + Low Rank](https://arxiv.org/abs/1705.07474)], [[Random Projection Trees](https://cseweb.ucsd.edu/~dasgupta/papers/rptree-stoc.pdf)],[[LargeVis](https://arxiv.org/abs/1602.00370)] | [[Lecture 2 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture2_public.pdf)] | [[graph tools for python](https://github.com/KrishnaswamyLab/graphtools)] |
|Monday January 17, 2022| **No class for MLK Day, and no regular office hours today. Please email me to set up a meeting for anything urgent.** |
|Wednesday January 19, 2022|Overflow from last time introducing the diffusion point of view of graph laplacian ; building graphs from data; Graph Partitioning Fundamentals| [[Module Detection Benchmarking in Biological Data](https://www.nature.com/articles/s41592-019-0509-5)], [[BigClam](https://cs.stanford.edu/people/jure/pubs/bigclam-wsdm13.pdf)], [[SBM for single-cell](https://link.springer.com/article/10.1186/s12859-021-04489-7)] | [[Lecture 3 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture3_public.pdf)] | [[LargeVis](https://github.com/lferry007/LargeVis)]  |
|Monday January 24, 2022| Graph Partitioning (Modularity-Based {Louvain, Leiden}; Finding disease-relevant modules from protein-protein and/or gene-gene interactions networks | [[Fast Unfolding of Communities in Large Networks](https://arxiv.org/abs/0803.0476)] | [[Lecture 4 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture4_public.pdf)]  | [[SNAP](https://snap.stanford.edu/)], [[Louvain](https://github.com/vtraag/louvain-igraph)], [[Leiden](https://github.com/vtraag/leidenalg)], [[graph-tool (SBM)](https://graph-tool.skewed.de/)] |
|Wednesday January 26| Finish probabilistic graph partitioning {SBM, Affiliation Model}); Graph Embeddings with node2vec (such as node2vec);  Single-Cell Day 1 : Intro to Single-Cell Profiling and Data Structures  | [[Node2Vec](https://dl.acm.org/doi/pdf/10.1145/2939672.2939754?casa_token=vQTboPUL6qIAAAAA:XQsAUtXd4MyWfj1ClUBw8FKhuPbpqO-aE2d7EDs5iX9-jJZP9BuxDbKUjg3CM69YKHALjCAKJtJx)], [[Representation Learning on Graphs](https://arxiv.org/abs/1709.05584)], [[Review: Graph Embedding in Comp Bio](https://www.frontiersin.org/articles/10.3389/fgene.2019.00381/full)], [[Vicus](https://journals.plos.org/ploscompbiol/article/authors?id=10.1371/journal.pcbi.1005621)] , **omitted for lack of time, but will come back to later (Graph Signal Processing (GSP) Basics**[[Intro to Graph Signal Processing in Machine Learning](https://web.media.mit.edu/~xdong/paper/spm20.pdf)] | [[Lecture 5 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture5_public.pdf)] | [[node2vec](https://github.com/aditya-grover/node2vec)] | 
|Monday January 31| Single Cell Day 1: Intro to Single-Cell {Data Structure, Technologies, Pre-Processing}, Automating Gating and Cell-Population Discovery in Single Cell Data| [[Spade](https://www.nature.com/articles/nbt.1991)], [[Single-Cells, Many Features](https://www.sciencedirect.com/science/article/pii/S009286741630410X)] | [[Lecture 6 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture6_public.pdf)]  | [[FCS file tutorial](https://github.com/stanleyn/fcs_tutorial)], [[Spade](https://github.com/nolanlab/spade)]   |
|Wednesday February 2| Graph-based automated gating, imputation in single-cell data|  [[phenograph](https://www.sciencedirect.com/science/article/pii/S0092867415006376)] | [[Lecture 7 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture7_public.pdf)] | [[phenograph](https://github.com/JinmiaoChenLab/Rphenograph)],  [[FastPG](https://github.com/sararselitsky/FastPG)] |
|Monday February 7| Imputation for single-cell data, Branch Preserving Visualization for Single-Cell Data| [[MAGIC](https://www.biorxiv.org/content/10.1101/111591v1)],[[PHATE](https://www.nature.com/articles/s41587-019-0336-3)],  | [[Lecture 8 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture8_public.pdf)] |   [[MAGIC](https://github.com/KrishnaswamyLab/MAGIC)],[[Phate](https://github.com/KrishnaswamyLab/PHATE)]  | 
|Wednesday February 9 [[*Homework 1 Assigned*](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/tree/main/Homework1)]| Branch Preserving Visualizating for Cellular Differentiation, Data Augmentation for Single Cell Identifying prototypical cells of a particular experimental condition with graph signal processing| [[SUGAR](https://papers.nips.cc/paper/2018/hash/c8ed21db4f678f3b13b9d5ee16489088-Abstract.html)] | [[Lecture 9 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture9_public.pdf)] | [[sugar](https://github.com/stanleyjs/sugar)] | 
|Monday February 14| Finish data augmentation for sparse single-cell landscapes, start graph signal processing background|[[Graph Signal Processing Review Article](https://web.media.mit.edu/~xdong/paper/spm20.pdf)],[[MELD](https://www.biorxiv.org/content/10.1101/532846v4)] | [[Lecture 10 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture10_public.pdf)] | [[MELD](https://github.com/KrishnaswamyLab/MELD)] [[pyGSP](https://pygsp.readthedocs.io/en/stable/)] |
|Wednesday February 16 [[*Project Proposal Signup Sheet*](https://docs.google.com/spreadsheets/d/1fX52jKWDWbJO1iB6D7FHv1DNQ53LPs0S8yNCUnUbSwQ/edit?usp=sharing)] ; [[*Project Proposal Template*](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Project_Proposal/Project_Proposal.pdf)] | Finish introducing graph signal processing, low-pass filtering, MELD for selecting condition-specific prototypical cells | See references from Monday. Also, [[The Emerging Field of Graph Signal Processing](https://arxiv.org/abs/1211.0053)] | [[Lecture 11 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture11_public.pdf)] | |
|Monday February 21| Finish up GSP background, Identifying condition or experimentally-specific prototypical cells with Meld, Start Differential Abundance Analysis with Cydar | [[Cydar](https://www.nature.com/articles/nmeth.4295)] | [[Lecture 12 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture12_public.pdf)] | [[cydar](https://www.bioconductor.org/packages/release/bioc/html/cydar.html)] |
|Wednesday February 23, **Homework 1 is due by 11:59pm eastern time on February 25**| Differential Abundance Day 2. Cydar,  Milo| [[Milo](https://www.nature.com/articles/s41587-021-01033-z)] | [[Lecture 13 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture13_public.pdf)] |  [[Milo](https://github.com/emdann/milopy)] | 
|Monday February 28 [[*Please sign up for your project presentations here!*](https://docs.google.com/spreadsheets/d/1fX52jKWDWbJO1iB6D7FHv1DNQ53LPs0S8yNCUnUbSwQ/edit?usp=sharing)]| Finish differential abundance analysis (Milo and Cydar), Contrastive PCA for dealing with background data | [[Contrastive PCA](https://www.nature.com/articles/s41467-018-04608-8)] | [[Lecture 14 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture14_public.pdf)]  | [[Contrastive PCA](https://github.com/abidlabs/contrastive)] |
|Wednesday March 2 **Please bring your laptops to class!**| Trajectory inference - guest lecture and tutorial by Jolene Ranek | [[PAGA](https://link.springer.com/article/10.1186/s13059-019-1663-x)], [[A Comparison of Single-Cell Trajectory Inference Methods](https://www.nature.com/articles/s41587-019-0071-9)], [[Slingshot](https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-018-4772-0)]. | [[Lecture 15 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture15_public.pdf)], [[Colab Notebook for trajectory inference](https://colab.research.google.com/drive/14LRc76ltDEnHi4v2jUWCS9Tad-RbXOLz?usp=sharing)] | [[PAGA](https://scanpy.readthedocs.io/en/stable/generated/scanpy.tl.paga.html)] | 
|Monday, March 7| Batch 1 of project presentations | [[Link to Presentation Schedule](https://docs.google.com/spreadsheets/d/1fX52jKWDWbJO1iB6D7FHv1DNQ53LPs0S8yNCUnUbSwQ/edit?usp=sharing)] |
|Wednesday, March 9| Batch 2 of project presentations | [[Link to Presentation Schedule](https://docs.google.com/spreadsheets/d/1fX52jKWDWbJO1iB6D7FHv1DNQ53LPs0S8yNCUnUbSwQ/edit?usp=sharing)] |
|Monday, March 14| Spring Break -- No class! |
|Wednesday, March 16| Spring Break -- No class! | 
|Monday, March 21| Finish differential abundance analysis (Milo), Contrastive PCA, Merging Multiple Single-Cell Datasets (Conos) | [[Conos](https://www.nature.com/articles/s41592-019-0466-z)] | [[Lecture 18 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture18.pdf)] | [[Conos](https://github.com/kharchenkolab/conos)] |
| Wednesday, March 23| Pseudotime, Diffusion, and Cellular Differentiation | [[Diffusion Maps for Differentiation](https://academic.oup.com/bioinformatics/article/31/18/2989/241305)], [[SLICER-developed at UNC](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-016-0975-3)], [[Original Diffusion Maps (Coifman)](https://papers.nips.cc/paper/2005/file/2a0f97f81755e2878b264adf39cba68e-Paper.pdf)] | [[Lecture 19 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture19_public.pdf)] | [[Diffusion Maps -Scanpy](https://scanpy.readthedocs.io/en/latest/api/scanpy.tl.diffmap.html)], [[SLICER](https://github.com/jw156605/SLICER)]  | 
|Monday, March 28| Last single-cell lecture. Branching trajectories with SLICER. Begin combining biological data from multiple modalities using Grassmann Embeddding| [[Subspace Merging on Grassmann Manifold](https://academic.oup.com/bioinformatics/article/35/10/1653/5134062?login=true)], [[Rayleigh Ritz Business (Spectral Clustering...](https://arxiv.org/abs/0711.0189)] | [[Lecture 20 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture20_public.pdf)] | [[Grassmann Cluster](https://github.com/michaelsharpnack/GrassmannCluster)] | 
|Wednesday, March 30| Finish multimodal data integration with Grassmann + Rayleigh Ritz, Start MOFA integration | [[MOFA](https://www.embopress.org/doi/full/10.15252/msb.20178124)], [[MOFA+](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-020-02015-1)] | [[Lecture 21 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture21_public.pdf)] | [[MOFA](https://github.com/bioFAM/MOFA)] |
|Monday, April 4| Integrating multiple heterogeneous graphs (e.g. multiple relational definitions) | [[Mashup](https://www.cell.com/cell-systems/fulltext/S2405-4712(16)30360-X?)] | [[Lecture 22 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture22_public.pdf)]  | [[Mashup](http://cb.csail.mit.edu/cb/mashup/)] | 
|Wednesday, April 6 [[*Project Presentation Signup* ](https://docs.google.com/spreadsheets/d/1_z1NBffJF8do8JrasTQl-8pS-ATR2ScI7SutRDPIf80/edit?usp=sharing)], [[*Final Project Writeup Template*](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/tree/main/Project_Final_Writeup)], [[**Homework 2 Assigned and due Fri April 22**](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/tree/main/Homework2)]| Graph Alignment and Summarization| [[REGAL (graph alignment)](https://gemslab.github.io/papers/heimann-2018-regal.pdf)], [[Refining Network Alignment](https://gemslab.github.io/papers/heimann-2021-RefiNA.pdf)] | [[Lecture 23 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture23_public.pdf)]  | [[REGAL](https://github.com/GemsLab/REGAL)], [[RefiNA](https://github.com/GemsLab/RefiNA)] |
|Monday, April 11| Graph Alignment Refinment, Summarization, and Compression | See papers from last time | [[Lecture 24 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture24_public.pdf)]|
|Wednesday, April 13| Label Propagation and Graph Neural Networks   | [[Correct and Smooth](https://arxiv.org/abs/2010.13993)] | [[Lecture 25 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture25_public.pdf)] |
|Monday, April 18, [[Project Rubric](https://docs.google.com/document/d/1FKh4_9VK6CHwqLs2V3mTo457FwELEFYNrXwEqNbGlBk/edit?usp=sharing)]| Imaging Modalities and Spatial Regularization | [[LEAPH](https://www.cell.com/cell-reports-methods/pdfExtended/S2667-2375(21)00124-7)] | [Lecture 26 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture26_public.pdf)] | 
|Wednesday, April 20| Technical Writing in Comp Bio and Wrap-Up, Summary of the Semester wrt to graphs in biomedicine | [[Watch : How to be a Machine Learning Biologist](https://www.youtube.com/watch?v=xueh6WnpRDQ&t=1651s)], [[Graph Representation Learning in Biomedicine](https://arxiv.org/abs/2104.04883)] | [Lecture 27 Notes](https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Lecture_Notes/Lecture27_public.pdf)] |
|Monday, April 25 [**zoom option available**]| Project Presentations Day 1 |
|Wednesday, April 27 [**No zoom option today**]| Project Presentations Day 2|
|May 5| Final Project Writeups Due

# Key Dates

* **Homework 1 Due:** February 23 (assigned by February 9)
* **Project Proposal Due:** March 9
* **Homework 2 Due:** April 20
* **Final Project Due:** Final Exam Day (May 5)

# Homework, Project, Reading, Grading, Etc

## Homework
There will be two homework assignments to practice implementing particular concepts. Often, things can become a bit easier to understand and use when they are implemented by you. I will provide code and hints in Python, but will be happy to read/run code written in Python, R, Julia, or Matlab. Please submit your homework writeup as a PDF. 

## Background Resources
Most of what we discuss in class will come from papers. However, I suggest the following textbooks as background references. Conveniently, they are also available for free.

* [PRML] Pattern Recognition and Machine Learning-- Chris Bishop [[Link](http://users.isr.ist.utl.pt/~wurmd/Livros/school/Bishop%20-%20Pattern%20Recognition%20And%20Machine%20Learning%20-%20Springer%20%202006.pdf)]

* [SLMP] Spectral Learning on Matrices and Tensors -- Majid Janzamin et al. [[Link](https://arxiv.org/abs/2004.07984)]

* The Matrix Cookbook [[Link](https://www.math.uwaterloo.ca/~hwolkowi/matrixcookbook.pdf)]

* [PML] Probabilistic Machine Learning: An Introduction. -- Kevin Murphy [[Link](https://probml.github.io/pml-book/book1.html)]

* [GRL] Graph Representation Learning -- William Hamilton [[Link](https://www.cs.mcgill.ca/~wlh/grl_book/)

* My favorite general linear Algebra Resource: Matrix Computational by Golub and Van Loan


## Readings
Each student much choose two class meetings to answer reading questions for one of the discussed papers. Please answer the following questions and send the responses in PDF format to me by the beginning of our class meeting. 

### Reading Questions

**Please choose 2 papers over the course of the semester to do this for, and turn them in before our class meeting 9:30 am to natalies+comp790@cs.unc.edu**. 

1) Please explain in 2 sentences or less what the problem being solved is.

2) What were the main contributions of the authors in this work? (You can answer in a few bullet points). 

3) Please describe 1-2 computational experiments that the authors implemented to test their method.

4) Were the authors the first to attempt this particular problem? If not, did they compare their results to other baselines? Do you think that their evaluation was objective?

5) Do you think that the authors provided enough evidence for why their developed method is an important contribution? If yes, please describe their reasoning here. If you do not think they adequately justified why they worked on this particular problem, please describe your thoughts on that here. 

6) What is one follow-up idea or extension from this work? 

## Final Project
I will provide you with several examples of publicly available biological datasets and problems (https://github.com/natalies-teaching/Comp790-166-CompBio-Spring2022/blob/main/Datasets.md). Half-way through the semester, you will submit your project proposal and present your idea to the class.  The proposal will be a short document describing 1) The problem 2) A background on other people's attempts to solve this problem and 3) A background on your idea of a solution and 4) the data you will use to test your method. At the end of the semester you will write a short paper explaining your method and results and present your results.

## Grading
 Grading will be based on the following

1) Reading Questions : 15% -- sufficiently 2 completed during the semester
2) Homework 1: 20%
3) Homework 2: 20%
4) Project Proposal : 10%
5) Project final writeup: 30%
6) Class Participation and Attendance : 5%

## Lateness Policy

I understand if things come up. If you need more time on your homework or project proposal, you are welcome to talk to me about it. However, if you simply turn in your homework late without any prior notice, I will deduct 10% of the points per day. There will be no late submissions of the course project permitted. 

## Mask Usage

I don't anticipate any problems with this, but if you do intent to join the class in-person, please make sure to wear a face mask covering your nose and mouth. 

## Accessibility Statement
The University of North Carolina at Chapel Hill facilitates the implementation of reasonable accommodations, including resources and services, for students with disabilities, chronic medical conditions, a temporary disability or pregnancy complications resulting in barriers to fully accessing University courses, programs and activities.
Accommodations are determined through the Office of Accessibility Resources and Service (ARS) for individuals with documented qualifying disabilities in accordance with applicable state and federal laws. See the ARS Website for contact information: https://ars.unc.edu or email ars@unc.edu.

(source: https://ars.unc.edu/faculty-staff/syllabus-statement)

## Diversity Statement
I value the perspectives of individuals from all backgrounds reflecting the diversity of our students. I broadly define diversity to include race, gender identity, national origin, ethnicity, religion, social class, age, sexual orientation, political background, and physical and learning ability. I strive to make this classroom an inclusive space for all students. Please let me know if there is anything I can do to improve, I appreciate suggestions.


