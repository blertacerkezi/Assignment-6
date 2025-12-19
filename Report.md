Assignment 6 Solution
---------------------

# Team Members
Lena Högger
Blerta Cerkezi

# GitHub link to your (forked) repository
https://github.com/blertacerkezi/Assignment-6


# Task 1

1. Indicate WebIDs of the group members and the files corresponding to the profiles of the group members.

Ans:
The group consists of the following members and WebIDs:

Blerta Cerkezi
WebID: https://wiser-solid-xi.interactions.ics.unisg.ch/bc/profile/card#me
Profile file: https://wiser-solid-xi.interactions.ics.unisg.ch/bc/profile/card

Lena Högger
WebID: https://wiser-solid-xi.interactions.ics.unisg.ch/lenahoegger/profile/card#me
Profile file: https://wiser-solid-xi.interactions.ics.unisg.ch/lenahoegger/profile/card


2. Indicate the URL of group profile and the file that contains the group profile.

Ans:

The group profile is represented as a FOAF group and is stored as a Turtle document in a Solid Pod.

Group profile URL (resource): https://wiser-solid-xi.interactions.ics.unisg.ch/b/group9.ttl#group
Group profile file (document): https://wiser-solid-xi.interactions.ics.unisg.ch/b/group9.ttl

The group profile contains FOAF statements defining the group and linking all group members via their WebIDs. 
The document is publicly readable via its Access Control List.
 



# Task 2

1. Create a SPARQL query to retrieve the URI of the group to which you belong from your FOAF profile. Provide the query in the [`query_group.rq`](query_group.rq) file. 


2. Query the names of all the people in your distributed social graph (i.e., people you know directly or indirectly) using your profile as an entry point. To do this, you will need to write a navigational query (see lecture slides) and use link traversal (using the command comunica-sparql-link-traversal). Try running the query without link traversal as well and see what happens. Provide the query in the [`query_friends.rq`](query_friends.rq) file (see project README) and explain the results.

Ans:




# Task 4

1. Which rules of Linked Data are applied to create the distributed knowledge graphs used in this assignment? Provide one concrete example for each rule you identify.

Ans: In this assignment, the following Linked Data rules are applied:

- Use URIs to identify things:
Each person and group is identified by a unique WebID (e.g. a Solid profile URL).

- Use HTTP URIs:
All WebIDs and resources can be accessed via HTTP in a browser.

- Provide useful information using RDF:
Profiles and groups are described using RDF and the FOAF ontology.

- Include links to other URIs:
Profiles link to other people and groups using properties such as foaf:knows and foaf:member.

2. One of your colleagues states that a Solid pod in itself is represented as a knowledge graph. Do you agree with this statement? Explain briefly

Ans: Yes, we agree with this statement.
A Solid pod stores data as RDF documents that consist of triples forming a graph structure. These graphs describe 
entities such as people, groups, and resources and their relationships, which matches the definition of a knowledge graph.

3. One core idea behind Solid is to decouple applications from data. Explain in your own words what this means and what technical and societal implications you see.

Ans: Decoupling applications from data means that users store their data in their own Solid Pods instead of in 
application-owned databases. Applications only access the data with the user’s permission.

Technically, this allows users to switch applications without moving their data. Societally, it gives users more 
control over their personal data and reduces dependency on large centralized platforms.

