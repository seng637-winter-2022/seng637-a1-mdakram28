# Lab. Report \#1 – Introduction to Testing and Defect Tracking
**SENG 637- Dependability and Reliability of Software Systems**

| Group \#:       | 34 |
|-----------------|---|
| **Student Names:** | Quinn Cooper |
|                 | Mohd Akram Ansari |
|                 | John Matthews Sarno |
|                 | Mahsa Malek |


**Table of Contents**

- [Introduction](#introduction)
- [Link of demo video](#link-of-demo-video)
- [High-level description of the exploratory testing plan](#high-level-description-of-the-exploratory-testing-plan)
- [Comparison of exploratory and manual functional testing](#comparison-of-exploratory-and-manual-functional-testing)
- [Notes and discussion of the peer reviews of defect reports](#notes-and-discussion-of-the-peer-reviews-of-defect-reports)
- [How the pair testing was managed and team work/effort was divided](#how-the-pair-testing-was-managed-and-team-workeffort-was-divided)
- [Difficulties encountered, challenges overcome, and lessons learned](#difficulties-encountered-challenges-overcome-and-lessons-learned)
- [Comments/feedback on the lab and lab document itself](#commentsfeedback-on-the-lab-and-lab-document-itself)




## Introduction

This report details our process, methodology and details of our testing of the ATM software. Before starting this assignment, we did not have any experience of software testing. All the methods used in his lab have been adapted from the content taught in SENG 637 and from the assignment description.  

The system under test is tested using three testing methods (in order)– Exploratory testing, Manual Functional Testing (MFT) and Regression Testing. Before starting the testing, we had no practical experience of these three types of testing. We just had a theoretical idea of the process. 

We will first perform exploratory testing which is a type of testing with no specific testing plan. We will work in pairs in this phase of testing, and we won’t be targeting any specific feature, rather, we will be randomly taking different paths in the software and trying out different features that are mentioned in the system requirements part in the assignment description. The plan used for exploratory testing is detailed in the next section of this report. 

Manual functional testing also tests each of the predefined functionalities one by one. The main difference is that this kind of testing is preplanned, and, in each step, we test specific documented functionality. The testcases that we will be testing are mentioned in detail in the assignment description. We will be following that exact plan in this phase of testing. 

Finally, we will also perform regression testing. It involves retesting all the features and bugs found in the previous stages for every new version of the SUT. In this case, we will test the ATM software version 1.1 using regression testing to check whether the bugs from version 1.0 have been fixed and what new bugs have been introduced. 

We divided our team into two pairs as it was required for exploratory testing: 

1. Quinn Cooper, Mahsa Malek 
2. John Matthews Sarno, Mohd Akram Ansari 



## High-level description of the exploratory testing plan

- Before starting exploratory testing understand the software requirements in detail to know exactly how the software is supposed to behave. 

- Perform initial testing from the standpoint of a customer who wants to achieve select goals (I.e withdraw $20, deposit money, etc.) 

  - Perform intensive feature testing on bugs that occur from initial testing 
  - Test the listed features with positive scenarios 
  - Test the listed features with negative scenarios (negative integers, unacceptable values, etc.) 

- Focus on critical features of the system like withdrawal, deposit, and PIN verification. 

- Feature Overview: 

  - **Operations:** 

    - System Startup 

    - System Shutdown 

    - Logs 

  - **Security/ User Verification:** 

    - Magnetic Card reader 

    - Card Pin Verification 

  - **Transactions:** 

    - Withdraw 

    - Deposit 

    - Transfer 

    - Inquiry 

- When a bug is identified, find out the scope of the bug. For example, if withdrawing $20 releases $40 from the ATM, then is that bug only specific to that amount or it happens no matter how much amount the user selects. 



## Comparison of exploratory and manual functional testing

The primary benefit we noted during our manual functional testing was the efficiency at testing edge cases. While MFT’s don’t cover all edge cases, when they are configured correctly, they do cover situations that would not come up in exploratory tests. 

One of the most obvious tradeoffs between exploratory and manual functional testing is the time commitment to go through the manual functional tests. Exploratory testing is much more freeform, whereas the check list approach of MFT can feel like a chore. However, this has a caveat, as the freedom afforded by exploratory testing can be overwhelming at times. 

An important advantage of the manual functional testing was the reproducibility of even the testcases which passed in the system. The exploratory testing wasn’t reproducible since the steps followed were not documented. The steps to rerun a scenario were documented only when a bug was found during exploratory testing. If we wanted to perform exploratory testing again, the testing would be completely different from the previous exploratory testing due to its random nature. 

The manageability of the MFT was also better than exploratory testing. Since each test case was clearly divided and documented, MFT was much easier to split between multiple testers thus making it much more efficient than exploratory test. We did not enjoy this advantage during exploratory testing which led to some redundant work between the testers. 

It’s hard to describe either of the two methods as more effective than one or the other because they both excel in conjunction with one another. Exploratory testing gives many ideas on how users actively interact with the software under test but it’s easy to overlook all the functions, whereas MFT gives comprehensive functional coverage but doesn’t give a good idea of how the system is actively interacted with. 



## Notes and discussion of the peer reviews of defect reports

The peer reviews of the bugs that we found consistently (between the two pairs) helped in improving the quality of the bugs that we found. Once a bug was found, it was verified by the other member of the pair and a considerable number of the times the bug was not actually a bug, rather, it was something expected from the system. The fresh perspective thus improved the quality of the bugs found. 

The other advantage of pair testing we found was higher quality bug reports. After the bug was verified by both members of the pair, we prepared the report of each bug collaboratively and this allowed us to increase the accuracy of the scope of the bug. A bug when found might affect some small feature of the software but, on further analysis and testing by multiple members revealed the exact span of the bug. Thus, we were able to create more accurate bug reports in this manner. 

One of the issues we faced when working in this manner was that when merging the work of both pairs, there were a few issues that were found by both the pairs, which proved to be redundant. But on the other hand, this also gave an idea of the higher importance of the bug and higher validity of the bug. 



## How the pair testing was managed and team work/effort was divided 

As mentioned in the impact of pair testing (previous section), team work directly improved the quality of our work. The increased collaboration allowed steady work progress too.  

The other important advantage of teamwork was that we were able to divide work according to the specialization of team members. For example, some of the team members were better at exploring the software under test while others were better at preparing reports. Identifying and utilizing the individual qualities of the team members enabled us to optimize the result of our collective efforts. 

Collaboration also helped us improve our understanding of the software requirements. When we discussed our understanding of the software requirements, all of us had a slightly different understanding of the requirements. After discussing the requirements in detail, we were able to refine our understanding of the requirements and thus we avoided adding unnecessary bugs to the issues backlog. 



## Difficulties encountered, challenges overcome, and lessons learned

One of the most pervasive issues we encountered in the assignment was the two peer review groups accidentally retreaded on each other's bugs found, so we accidentally repeated work. However, once we began listing bugs in backlog, we could easily see if a certain bug was already documented. 

The most pressing difficulty we encountered was that it is actually very difficult to succinctly explain a bug! When writing bug reports, it’s easy enough to detail how to replicate a bug and listing initial states, but when it came to titling the report, we couldn’t agree on how to explain it within a sentence. The exercise of titling the reports was great for building our communication skills, particularly given how important it is to convey that information quickly and correctly. 



## Comments/feedback on the lab and lab document itself

The document was highly detailed and had all the information that we needed to start testing the SUT. Along with having the explanation of the procedures that we had to follow for the different kinds of tests, the document also has a detailed explanation of the system requirements. 

The only issue that we found with the requirement was that it mentioned lab and in person work while SENG 637 is a web-based course and with no lab. But it wasn’t a challenge getting around that information as we figured that all the information relevant to the assignment was already mentioned in the document. 
