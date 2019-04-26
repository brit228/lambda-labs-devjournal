# Labs - Week 1 - Development Journal

## Part 1 - Individual Accomplishments this Sprint

I was able to create and deploy a Frontend, Backend and PostgreSQL Database application, which uses the
Google Maps API to generate a premilinary visualization of the geographic data. The data uploaded to the database
contains geometry information that can be read and processed by the PostGIS extension, so the containing geomtry for
a point can be determined. Other graphs/charts have been created on the Frontend, that visualize other aspects of the data.
I had difficulty in some of the aspects relating to PostGIS and the visualizations (was using d3.js, moved to nivo.rocks),
and have been primarily been using VS Code, local development servers, and PGAdmin4 for creating code, testing code, and
setting up a Database.

## Detailed Analysis

![Example map visualization.](samplemap.png)

## Part 2 - Milestone Reflections

It was hard for me to get going with Trello and GitHub, but I have now gotten into the rhythm of using both, Trello especially.
Because I do tend to go into my own world when writing code, and my current responsibilities are further detatched from the
other data scientists, I need to rely on Trello and GitHub more (or communicate better) to update my teammates. The other problem
that I have had, and am currently having, with team projects, is that I do tend to push my ideas and don't communicate effectively.
I often find that I have finished a solution to a problem that other people are working on that we have had no communication over.

So far, I have spent a lot of time researching the PostGIS in order to figure out how to get the approximate location of the
incident/crime to a local area. We have so far decided to go with census tract, which is small enough to get a more specific
area, without being too small to suffer from lack of data and too small for the user. PostGIS has been useful in that it is an
extension for the Database, and can be used to determine which geometry or census tract a point is contained by.
