# Automatic-Code-Cleaning-in-R-with-Rclean

The details of the codeset and plots are included in the attached Microsoft Word Document (.docx) file in this repository. 
You need to view the file in "Read Mode" to see the contents properly after downloading the same.

A Brief Introduction
=====================

The R language has become very popular among scientists and analysts
because it enables the rapid development of software and empowers
scientific investigation. However, regardless of the language used,
data analysis is usually complicated. Because of various project
complexities and time constraints, analytical software often reflects
these challenges. “What did I measure? What analyses are relevant to
the study? Do I need to transform the data? What’s the function for the
analysis I want to run?” Although many researchers see the value in
learning to write software, the time investment for learning a
programming language alone is still exceedingly high for many, let
alone also learning software best practices. The downside to the rapid
spread of data science is that learning to create good software takes
a back-seat to just writing code that will get the job “done” leading
to issues with transparency and software that is highly unstable
(i.e. buggy and not reproducible).

The goal of the R package Rclean 
is to provide a automated tool to help scientists more easily write
better code. Specifically, Rclean
has been designed to facilitate the isolation of the code needed to
produce one or more results, because more often then not, when someone
is writing an R script, the ultimate goal is analytical results for
inference, such as a set of statistical analyses and associated
figures and tables. As the investigative process is inherently
iterative, this set of results is nearly always a subset of a much
larger set of possible ways to explore a dataset. There are many
statistical tests and visualizations and other representations that
can be employed in a myriad of ways depending on how the data are
processed. This commonly leads to lengthy, complicated scripts from
which researchers manually subset results, but which are likely never
to be refactored because of the difficulty in disentangling the code.

The Rclean package uses a
technique based on data provenance and network algorithms to isolate
code for a desired result automatically. The intent is to ease
refactoring for scientists that use R but do not have formal training
in software design and specifically with the “art” of creating clean
code, which in part is the development of an intuitive sense of how
code is and/or should be organized. However, manually culling code is
tedious and potentially leads to errors regardless of the level of
expertise a coder might have; therefore, we see
Rclean as a useful tool for
programming in R at any level of ability. Here, we’ll cover
details on the implementation and design of the package, a general
example of how it can be used and thoughts on its future development.
