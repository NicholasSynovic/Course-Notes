# Week 1
- Project Name (Tenative): PoliPy
- Goal: To develop a program that maps the relationships that different Congressional Representatives share and have across the large breadth of legislature hosted on Congress.gov
- Utilized Tools: Neo4J and Python Latest
- Personal State of Purpose: To make understanding the inherit relationships that occurn in Congress appearent to constituents

# [Neo4J Information](https://neo4j.com/)
- Will start off using the Neo4J Native Graph database to store information
    - Will use other tools offered by the platform potentially later to display the information

# Python Latest information
- Will try to use the Python XML Parser for the purpose of anlyzing the contents of legislature
- Will be working on a seperate feature outside of this research as a weekend project to create a SQL database of all the legislature hosted on Congress.gov

# [Neo4J Graph Data Science for Dummies](https://neo4j.com/graph-data-science-for-dummies)

# Initial Analysis on Feasibility to Solely Use XML Data to Accomplish Goal
- Infeasible off of preliminary analysis conducted on January 22 12:02 AM
    - Information provided covers what the bill wants to make into law
    - Very basic meta data about the bill itself
        - Information on who created the bill, the committee assigned to the bill, and so on
        - More information can be found in the Congress.gov overview of the bill
    - More research needs to be done into other bills at various stages of passing through Congress for feasibility to be confirmed or denied
    - NOTE: I am worried that this research will involve having to create a Congress.gov web scraper. A fairly large task, however, it would provide all of the data for a given Congress session. I'll work on this over the weekend.
