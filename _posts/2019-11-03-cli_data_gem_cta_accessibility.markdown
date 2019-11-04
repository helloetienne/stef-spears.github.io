---
layout: post
title:      "CLI Data Gem: CTA Accessibility"
date:       2019-11-04 01:09:50 +0000
permalink:  cli_data_gem_cta_accessibility
---


My data gem project is a simple interface to determine whether a particular Chicago Transit Blue Line station is ADA accessible. My original plan was to give the user the option to type in the name of a train line (Red, Blue, Green etc) and then the program would give the user options to find whether the train was "delayed" or "on time". However, I quickly realized this wasn't feasible for the scope of my project due to the manner in which the CTA provides this information and the level of familiarity I currently have with using live data. I accessed the City of Chicago data portal, and used an API called "CTA - System Information - List of 'L' Stops". The API gives a list of attributes like "stop ID", "station name", and flags for the color name of the train, among other options. I chose to pull the "ada" attribute for my project.

When the program is called, the user receives a greeting and a list of train stations. The user then types in the name of a station, or "exit". If the program receives a valid station name, it returns the ADA info for that station. Otherwise it prompts the user to modify their answer.

I created a branch of this project to attempt to add another layer of functionality to the program, however I was unable to get the code clean and working in time for submission. On this separate branch, I attempted to first have the program give the user multiple train selection options, and then have the user select a train station from there. I hope to build out this functionality for this program in the future, however the current iteration of my program cleanly does what it sets out to do.
