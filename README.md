# tb.lx Tech Radar

tb.lx Tech Radar is our technology portfolio management tool. It reflects both established and emerging technologies being evaluated, adopted, or deprecated within our company. This tool supports teams in choosing the right technologies for future products and projects, fostering informed and consistent decision-making.

Our Tech Radar concept draws inspiration from ThoughtWorks, and their well-known Technology Radar. In addition, our project builds upon the open-source tech-radar project developed by [AOE](https://github.com/AOEpeople/aoe_technology_radar) under the Apache License.

You can access our tech radar [here.](https://tblxio.github.io/tech-radar/)

## Workflow
The tech radar is built on data entries specified in `/radar`.<br />
Below you find the ID(s) related to each status (ring) and category (quadrant):

| Ring       | ID       |
|------------|----------|
| Adopt      | `adopt`  |
| Trial      | `trial`  |
| Assess     | `assess` |
| Hold       | `hold`   |


| Quadrant                    | ID                              |
|-----------------------------|---------------------------------|
| Languages & Frameworks      | `languages-and-frameworks`      |
| Platforms & Infrastructure  | `platforms-and-infrastructure`  |
| Developer Tools             | `developer-tools`               |
| Methods & Patterns          | `methods-and-patterns`          |


### Setting up new data
For a new entry, create a folder under `/radar/{date-of-entry}` with the name of the technology. The entry files must be in Markdown format (.md). Each file has a front-matter header with the attributes of the technology. E.g.:

```
---
title: React
quadrant: languages-and-frameworks
ring: adopt
tags: [frontend] <!--- tags are optional --->
---

# React 

Description and context goes here.

[Link to ADR].
```

## Setup

  ### Prerequisites
  - [Node.js](https://nodejs.org/en/)
  - [yarn](https://classic.yarnpkg.com/en/docs/install/)

  ### Installation
  - clone the repo
  - `yarn` for dependencies installation

  ### Commands
  - `yarn build` for building the initial tech radar
  - `yarn dev` for launching the development server


## Versioning
  
We use [SemVer](http://semver.org/) for versioning.


## Licensing
This project is released under the MIT License. It depends on the code and ideas from the AOE tech-radar project © AOE GmbH.
