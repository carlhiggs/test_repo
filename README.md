--- 
# A YAML template for project metadata
# inspired by https://github.com/leipzig/metadata-in-rcr/blob/master/data/examples/rescience_metadata.yaml
# Carl Higgs 2021

# Project name
title: "Project name" 

# List of team members with name, affiliation, orcid, and project role
# Affiliation "*" means primary contact for this project
team:
   - name: Your Name
     affiliation: 1*
     orcid: Your ORCID 
     role: Project lead
     e-mail: your.name@rmit.edu.au
   - name: "Your co-author's name" 
     affiliation: 1
     orcid: Their ORCID 
     role: Geospatial analyst
     e-mail: ~
   - name: "Your other co-author's name" 
     affiliation: 2
     orcid: Their ORCID 
     role: Dungeon master
     e-mail: ~

# List of affiliations with code (corresponding to author affiliations), name
# and address. You can also use these affiliations to add text such as "Equal
# contributions" as name (with no address).
affiliations:
  - code:    1
    name:    Healthy Liveable Cities Lab, RMIT University
    address: Melbourne, Australia
  - code:    2
    name:    School of Computing Technologies, RMIT University
    address: Melbourne, Australia


# A list of keywords, could include Field of Research terms (or that could be a seperate entry?)
# Could also include
keywords: [Built environment and planning, Epidemiology, Agent-based Modelling, Python]   


# Project description (the bar character "|" allows for multi line entry
abstract: | 
    Background
    A Lorum ipsom very interesting context to this project is...
    
    Aim
    To use words which sound like sentences, and demonstrate blahhdhdhdh
    
    Methods
    We use a range of dklaffjdaflkdja flka
    
    Outputs
    Project ouputs will be disseminated as aldjkflkajlfkjdalkfjladj


# Project start date, and where applicable, end date
start-date: YYYY-MM-DD
end-date: ~


# Code URL, DOI and licence
# use SPDX identifiers, see https://spdx.org/licenses/
code:
  - url: 
  - doi:
  - licence:

# Data URL, DOI and licence
# Pre-pend data with * to indicate output dataset(s) of this project 
# URL may be a file path which is not publicly accessible
# use SPDX identifiers, see https://spdx.org/licenses/
data:
  - dataset: Data name
    url:  # this may be a file path which is not publicly accessible
    doi:
    licence:
    role: what role this data played
  - dataset: Another dataset name which happend to be an output*
    url:  
    doi:
    licence:
    role: A modelled dataset produced through this project
  
# Study region(s)
# include a descriptive name (eg city, country), time point, and explicit bounding box
# time may be single year, a list of years [YYYY,YYYY], or range of years [YYYY:YYYY]
# more specific time points such as ranges of months or days can be used, 
# eg [YYYY-MM:YYYY-MM] or [YYYY-MM-DD:YYYY-MM-DD]
locations: # draw CSV bbox for region(s) at https://boundingbox.klokantech.com/, and place in square brackets
   - region:    Melbourne, Australia
     bbox:      [144.657982,-38.190588,145.444878,-37.564056] 
     timepoint: 2012 
   - region:    Bogota, Colombia
     bbox:      [-74.223689,4.4604,-73.996423,4.837015] 
     timepoint: [2012,2016]
---

# Markdown with YAML header test

This is a test of a markdown document with a YAML header for metadata, visualising how this might look.  In this section regular markdown could be used to describe a project and its aims.

Aims might include:

 - to A
 - to B
 - to C

A timeline could be included

|Start     |End        | Description|
|----------|-----------|-------------|
|2020-10-05|2023-01-30 | This is a time window when something could happen|
|2021-11-05|2022-01-30 | Another duration|
|2023-01-01|2023-01-23 | Something else|

To find out more contact a.person@someplace.org
