+++
showonlyimage = false
image = "img/portfolio/sensu_docs_home.png"
date = "2022-11-30T19:44:32+05:30"
title = "Sensu Documentation"
weight = 1
+++

I wrote and edited Sensu's documentation, including API documentation, references, and user guides. I also maintained and improved the Hugo docs site and reworked the information architecture.

<!--more-->

[Sensu](https://sensu.io/) is an agent-based monitoring and observability tool that you install on your organization’s infrastructure. Sensu users can collect status events and metrics, configure context-rich alerts that improve incident response and reduce alert fatigue, and transmit collected data to long-term storage. 

I wrote and edited Sensu's documentation as the sole technical writer for 3 years. I also maintained the Hugo docs site, reworked the docs site's information architecture, redesigned the docs landing page, notified customers of new and updated documentation, and developed Katacoda scenarios to help people learn Sensu.

### Work examples

Sensu's documentation is published at [https://docs.sensu.io/](https://docs.sensu.io/). Here are some examples that demonstrate my work:

* API documentation:
	* [core/v2/checks](https://docs.sensu.io/sensu-go/latest/api/core/checks/)
	* [core/v2/entities](https://docs.sensu.io/sensu-go/latest/api/core/entities/)
	* [enterprise/pipeline/v1](https://docs.sensu.io/sensu-go/latest/api/enterprise/pipeline/)
	* [enterprise/secrets/v1](https://docs.sensu.io/sensu-go/latest/api/enterprise/secrets/)
* References:
	* [Checks reference](https://docs.sensu.io/sensu-go/latest/observability-pipeline/observe-schedule/checks/)
	* [Entities reference](https://docs.sensu.io/sensu-go/latest/observability-pipeline/observe-entities/entities/)
	* [Pipelines reference](https://docs.sensu.io/sensu-go/latest/observability-pipeline/observe-process/pipelines/)
	* [Secrets reference](https://docs.sensu.io/sensu-go/latest/operations/manage-secrets/secrets/)
* Guides:
	* [Install Sensu](https://docs.sensu.io/sensu-go/latest/operations/deploy-sensu/install-sensu/)
	* [Collect service metrics with Sensu checks](https://docs.sensu.io/sensu-go/latest/observability-pipeline/observe-schedule/collect-metrics-with-checks/)
	* [Reduce alert fatigue with event filters](https://docs.sensu.io/sensu-go/latest/observability-pipeline/observe-filter/reduce-alert-fatigue/)
	* [Send Slack alerts with a pipeline](https://docs.sensu.io/sensu-go/latest/observability-pipeline/observe-process/send-slack-alerts/)
	* [Use secrets management in Sensu](https://docs.sensu.io/sensu-go/latest/operations/manage-secrets/secrets-management/)
	* [Create limited service accounts](https://docs.sensu.io/sensu-go/latest/operations/control-access/create-limited-service-accounts/)
	* [Configure integrations in the Sensu Catalog](https://docs.sensu.io/sensu-go/latest/catalog/sensu-catalog/)
	* [Set environment variables with sensuctl](https://docs.sensu.io/sensu-go/latest/sensuctl/environment-variables/)
* [Troubleshoot Sensu](https://docs.sensu.io/sensu-go/latest/operations/maintain-sensu/troubleshoot/)

I worked with Sensu's engineers, product manager, and support and sales teams to identify documentation needs and track down source material. OpenAPI Specification files and the API source code were available as source material for the API documentation, and I tested and confirmed API calls and responses with Postman. To develop and test the docs as I worked, I ran Sensu in Vagrant boxes and Docker containers.

When someone else on the Sensu team drafted docs content, I helped them test and edit it as well as find the right spot for it within the docs site.

### Hugo docs site

The docs were deployed to a Hugo site. I did not create the site, but I maintained it and added improvements as needed:

* Updated Hugo and dependencies
* Migrated to a new version of Algolia for search
* Added shortcodes for automatic lists and partials for alert banners
* Added a basic feedback mechanism that sent results to Google Analytics

### Information architecture project

To support Sensu's transition to a single product, I completed a project to rework the docs site's information architecture so that it aligned with the new product and the Sensu Observability Pipeline concept. I followed the approach described in [Everyday Information Architecture](https://everydayia.com/) by Lisa Maria Martin to complete an audit, categorize the content, and sort out the structure and navigation. Then, I worked with my boss to refine the new structure and incorporate feedback from every team.

After the plans were finalized and approved, I created a Trello board to organize, prioritize, and track the reorganization work. I broke the work down into logical groups of tasks and created a Trello card for each task to make sure I didn't overlook anything---every page in the docs was affected. As I worked, the Trello board was handy for quickly communicating the project status. As I completed each group of tasks, I used Slack to explain the changes internally and posted to the Sensu Community Forum to explain the changes to our customers.

In the course of the information architecture project, I used Lucidchart to design and create an [interactive SVG image of the Sensu Observability Pipeline](https://docs.sensu.io/sensu-go/latest/) to give customers a mental model of how Sensu works. Readers can click any element in the pipeline image to get more information. I also set up a simple JavaScript button to simulate a "tour" through each element in the observability pipeline.

As the final piece of the project, I redesigned the docs landing page. We wanted the landing page to give people a quick overview of Sensu Go and demonstrate the breadth of documentation we offered. I wireframed the landing page in Lucidchart and again worked with my boss and other stakeholders to adjust the design until everyone was satisfied. I worked with a contractor to implement the new landing page.

### Tools

I used these tools in the course of my work on the Sensu documentation:

* Docker
* Git &#8226; GitHub
* Hugo
* Lucidchart
* Markdown
* OpenAPI Specification
* Postman
* Snagit
* Vagrant 

