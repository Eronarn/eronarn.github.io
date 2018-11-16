---
layout: post
title: Financial data pipelines at Quantopian (Quantopian Webinar)
---

I presented a webinar version of my Velocity New York presentation, this time titled _Financial data pipelines at Quantopian_. [Slides are available via Google Drive](https://drive.google.com/open?id=1wasIEUZAQpKx7mEga2r2Xvy31sjMogfipOmQ85cUlKo), or you can [watch the recording on YouTube](https://www.youtube.com/watch?v=81F8A6tHM30).

Here's the talk abstract:

_The Quantopian data pipeline begins every night after equity trading in the US ends when the company ingests the day’s financial data from several vendors. Its Python infrastructure reconciles and cleans data to produce a unified view of history, repackages cleaned data into higher-performance formats, and produces analytics data that is provided to Quantopian’s worldwide community as a free portfolio risk model (usually only available to institutions)._

_But that high-level view of Quantopian’s business is an abstraction; as the company scaled its research and trading infrastructure, the engine keeping Quantopian running grew to almost a hundred cron jobs. These brittle scheduling systems regularly failed in the real world, where vendors are late, data is missing, and services fail. As the company considered adding support for global markets, it knew it needed to invest in a more resilient and flexible approach._

_Quantopian began researching a data pipeline solution in late 2017 and rapidly converged on Apache Airflow as the right tool for the job. The team spent a month on research and prototyping and another month developing a detailed implementation plan to introduce Airflow to the rest of the company: adoption targets, documentation, code samples, and test suites._

_Quantopian’s site reliability engineer James Meickle explains how in less than six months, Quantopian went from not knowing how it would ever escape its cron jobs to putting Airflow on the critical path for its high-reliability trading infrastructure. And the best news? Since Quantopian has done the research for you, you can do it even faster._