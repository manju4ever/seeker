# Seeker

### This document would briefly explain the problem of the modern BI tooling landscape, high level implementation details, user personas, tools/frameworks/libraries to be used to build a self-serviceable BI tool. 

### Objective

Design a self-servicable Business Intelligence (BI) tool to support exploration, and visualiztion of enterprise level datasets. The solution should be highly robust, scalable, maintainable and high performing.


### The problem of multiple data sources and multiple data models

* The most challenging part of today's BI world is the ability to form a common dialect out of a variety of infromation storage systems. These systems can range from a simple file system to complex RDBMS based, document based, or object based data storage systems. 

### The need for Domain Specific Language (DSL) to tackle multiple formats of data

* The creation of DSL for applications in general seems to be increasing over the past few years. These DSL(s) can be seen in areas such as Oceanography, Meteorology, Quantum Computing, and many other fileds to provide an open format to process complex instructions behind the screens.

* One specific example of DSL used on the BI Field today which has seen enormous growth is LookML. LookML is the crux of Looker owned by Google.

LookML Reference: https://docs.looker.com/data-modeling/learning-lookml/what-is-lookml

### Key Terminology of the proposed solution

1. Pages
    - This is the section where the business user would select different data labels available to construct his own meaningful graph
    
2. Explore
    - This is the section where a Business Analyst typically creates meaningful Labels requested by the business
    - This section would use Feilds created from the Develop section
    
3. Develop
    - The section would be in an intermediate format (like LookML) with the use of DSL created to pick the necessary columns/fields from different data sources
    - This section will have complete versioning enabled to keep track of fields created
    
4. Configure
    - This is the section where the BI tool admin would configure connections to different data source. Read actual schemas from the DB's or otherwise
    - This also provided facility to manage Identity and Access Management to provided required level of access to the users.
    
    
### Available Open Source Solutions which almost provide features like above

1. Apache SuperSet
2. Metabase


### Available Commercial Solutions

1. Looker - https://looker.com/
2. ThoughtSpot - http://thoughtspot.com/
