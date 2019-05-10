# Sprint Challenge - Week 3

## Part 1 - Individual Accomplishments

- Styling: Imported and used Bootstrap on /map page, and have chosen fonts, colors, and designed/animated logo
- Redis: Changed where results are stored to Database, and automatically deletes rows over an hour long with job result queries.
- Prediction: Created Frontend & Backend functions for getting static predictions. Currently only the Date chart shows predictions.
  - Also helped Samir & Albert in designing prediction model and output for model.

## Detailed Analysis

[Backend Pull Request to Master](https://github.com/labs12-crime-statistics/Backend/pull/39)

- Addition of Redis:
  - Due to timeouts occurring on Heroku, jobs were run in separate Dyno with Redis acting as a job queue. The user would then make a
    request every 5 seconds to see if the job has been completed and to download the data from a database once it was done. This is
    as the result can be quite large, and should therefore not be stored in memory in Redis.
  - The python tools used for creating and searching for jobs on Redis is the python 

## Part 2 - Milestone Reflections

A lot of different services were looked at this week, including Google Maps Places API, for address autocomplete and reverse geocoding,
and Redis/Redis Queue. There were a lot issues with using these products, especially with trying to use AWS Elasticache for hosting the
Redis cluster, which had the issue of not being public initially, meaning that a NAT EC2 instance had to be created to transfer
information from the port requests to the Redis cluster. The Google Maps Places API had a few issues as well, mainly due to the fact that
errors were being returned without any explanation of what they meant.

I have been working better with Samir and Albert this week, especially in terms of designing the predictive models and everything. However,
because I am used to the current pace that I am working at, I am finding it difficult to delegate/share tasks related to the
Frontend/Backend. However, I am the only one with JS experience, and the Backend is pretty much complete, only some optimization and
documentation remains to be done on it, so there is only the Frontend to worry about.
