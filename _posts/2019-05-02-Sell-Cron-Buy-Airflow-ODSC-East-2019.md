---
layout: post
title: "Sell Cron, Buy Airflow: Modern data pipelines in finance (ODSC East 2019)"
---

I [presented at ODSC East 2019](https://odsc.com/training/portfolio/sell-cron-buy-airflow-modern-data-pipelines-in-finance) about Quantopian's use of [Apache Airflow](https://airflow.apache.org/) for our financial data pipelines. This is an update from my previous presentations on this topic to focus on our new Quantopian Alpha Model (QAM) system, which is built on Airflow. The [slides are available via Google Drive](https://docs.google.com/presentation/d/1Dw0pMqAQ3iQ7Gq_YHirL9pyHNVkGXr-96PnelAkXVyU/edit).

<!--more-->

Here's the talk abstract:

_Quantopian's data pipelines ingest financial data from vendors to produce a unified view of market history repackaged into high-performance formats. In 2018 we entered into a partnership with FactSet and began dramatically expanding the data available on our platform. We selected Apache Airflow as a workflow engine in order to cope with the additional complexity and maintain high availability for our production data systems._

_Our community of algorithm authors becomes more productive with every dataset we add to the platform, so we knew that we’d need to deploy new algorithms faster than ever before. In the latter half of 2018, we started building a new production system, the Quantopian Alpha Model (QAM), to allow our investment team to incorporate ideas from many more authors in our community._

_We decided to build QAM by applying proven DevOps methodologies like containerization and continuous deployment to data science fundamentals. QAM’s nightly pipeline leverages scientific Python for data processing, Kubernetes for execution, and Apache Airflow for orchestration. QAM is also entirely code-defined and shipped via pull request, allowing developers to perform mid-day code deployments with no involvement from operations._

_This development methodology has been a resounding success: our team of four went from creating a repo to placing live trades in three and a half months. Now that we’ve shipped QAM, we’d like to help you ship your data science projects faster, too._
