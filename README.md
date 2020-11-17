# Releng Agile Process Tracking

This repo contains documentation and issues related to how the Releng team at Mozilla runs its agile development process.

Based heavily on the [Taskcluster team's repo](https://github.com/taskcluster/scrum).

Table of Contents
=================

   * [Releng Agile Process Tracking](#releng-agile-process-tracking)
      * [Definitions](#definitions)
         * [Theme](#theme)
         * [Initiative](#initiative)
         * [Sprint](#sprint)
         * [Epic](#epic)
         * [Story](#Story)
         * [An Example](#an-example)
      * [Tools](#tools)
      * [Roles](#roles)
         * [1. Product owner](#1-product-owner)
             * [1a. Epic owner](#1a-epic-owner)
         * [2. Scrum master](#2-scrum-master)
         * [3. Future sprint champion](#3-future-sprint-champion)
      * [Sprint process](#sprint-process)
         * [Planning a sprint](#planning-a-sprint)
             * [Estimation](#estimation)
         * [Choosing the next sprint](#choosing-the-next-sprint)
         * [Workspace configuration](#workspace-configuration)
         * [Starting the sprint](#starting-the-sprint)
         * [During the sprint](#during-the-sprint)
         * [Ending the sprint](#ending-the-sprint)
         * [Time between sprints](#time-between-sprints)

______

## Definitions

In order to avoid confusion when discussing our process, it's helpful to define the various terms we use to categorize our work at different levels of granularity and how they roll up into each other.

We generally follow [the Atlassian model](https://www.atlassian.com/agile/project-management/epics-stories-themes).

Theme -> Initiative -> Sprint -> Epic -> Story (-> Subtask)

### Theme

A _theme_ is a large focus area than spans the Mozilla organization and is pertinent to and addressable by the Releng team. Themes are roughly analogous to organization objectives. Themes are gathered [here](https://github.com/mozilla-releng/scrum/blob/main/gen/themes.md).

### Initiative

An _initiative_ is a collection of one or more sprints that, taken together, address one or more themes. Initiatives map to major roadmap projects that the Releng team would like to accomplish, and can be either new functionality or substantial reworks of existing functionality. Depending on the project area, an initiative can be a thin wrapper around a single sprint if that sprint is high value and self-contained.  Initiatives are gathered [here](https://github.com/mozilla-releng/scrum/blob/main/gen/initiatives.md).

### Sprint
The _sprint_ is made up of a small collection of epics, and should be resolvable without a period of 2-5 weeks. This can be a thin wrapper around a single epic if the user story is large and/or important enough. Sprints can address one or more initiatives; all the epics in a given Sprint do not need to service the same initiative. Sprints are tracked [in Jira](https://jira.mozilla.com/secure/RapidBoard.jspa?rapidView=679&view=detail).

### Epic
An _epic_ is a collection of user stories that describes plainly a feature of Releng infrastructure.

### Story
A _story_ is a single, cohesive task as represented by a Jira story. Larger stories should be decomposed into smaller subtasks. No single story should take more than 1 engineer week to accomplish, modulo time to review and deploy. Stories should address a single epic.

A well-defined story is the basis for all of our estimation. It cannot be overstated how important it is to make sure tasks are decomposed to the point where they can be estimated accurately. It underpins _everything_ else.

### An Example

Here is a top-down categorization example from an actual sprint:

We should revisit this once we have clearer examples.

* Theme: Project Maintenance, User growth
* Initiative: Fenix with Shipit
* Sprint: Fenix with Shipit
* Epic: [Fenix with Shipit](https://jira.mozilla.com/browse/RELENG-6)
* Story: [Automatically version bump](https://jira.mozilla.com/browse/RELENG-74)

## Tools
All Releng work for sprints is tracked in Jira.

Sometimes [Bugzilla](https://bugzilla.mozilla.org) bugs or Github issues will be part of our sprint. When this happens we will create a corresponding story or Epic in Jira and reference the original bug or issue.

We are using [Jira](https://jira.mozilla.com/) to manage our agile process. Jira allows for:
* dependency tracking
* estimate tracking
* sprints
* burndown charts

Any issues that are purely process-based (e.g. scrum documentation) should be filed in [the scrum repo](https://github.com/mozilla-releng/scrum). Epics are represented in Jira as [specially-tagged issues](https://jira.mozilla.com/browse/RELENG-79?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20resolution%20%3D%20Unresolved%20ORDER%20BY%20priority%20DESC%2C%20updated%20DESC). Since they are a process abstraction to link issues together, Epic issues should be filed in the scrum repo as well.

## Roles
We have three defined roles in our agile process:

### 1. Product owner
The _Product owner_ manages the product backlog and keeps the rest of the team working on the most important thing. They have the final decision on matters of scope. They can also change the scope of the current sprint or, at their discretion, end the sprint early.

#### 1a. Epic owner
For sprints composed of multiple, unrelated epics, a different _Product owner_ can be assigned per epic.

### 2. Scrum master
The _Scrum master_ deals with the scrum process itself. They run the kick-off meetings, the daily stand-ups, and the wrap-up meetings (review & retrospective) for every sprint. They prompt developers for status and follow-up when developers are blocked. They support the Product owner in whatever way the Product owner deems necessary. The _Scrum master_ also works with _Future sprint champions_ to ensure high quality, well-scoped milestones for future sprints.

### 3. Future sprint champion
The _Future sprint champion_ is responsible for organizing issues in the Product Backlog into cohesive epics that the team can work towards in a future sprint. They are expected to devote a few hours every week to triaging issues in the backlog to refine the scope for the future sprint. Note: there can be multiple _Future sprint champions_ active at one time.

## Sprint process

### Planning a sprint
During the previous sprint, one or more Future sprint champions do the work organize the issues into epics, and epics into new sprints. User stories are discussed and converted into Epics. New issues are filed or existing issues are tagged against the upcoming sprint.

Zenhub allows setting dependencies between issues. While we need to be careful to avoid having _too many_ dependencies within a given sprint to avoid blocking work, we should leverage dependencies to help reveal the critical path for sprints.

When planning for upcoming sprints, we should focus on the needs of Releng and the community deployment. We can act on specific requests or use cases from the Firefox deployment, but we should not assume anything on their behalf. This will help avoid Mozilla-specific solutions and potential re-work later on.

As much as possible, [RFCs](https://github.com/mozilla-releng/releng-rfcs) should be written *outside* the sprint process, with only implementation happening within the context of sprints. If the amount of work required for implementation is unclear, estimates should be higher.

#### Estimation
The Releng team uses Fibonacci-scale story points for estimation. Each team member is assumed to be able to deliver on 3-4 story points in a given week. This gives individuals time to deal with interrupts and also to pursue some professional development time. Care should also be taken to plan around upcoming holidays and vacation to avoid over-packing the next sprint.

The first step for sprint estimation is adding up the available story points for all team members over the coming weeks to see what the maximum achievable amount of work is. Combined point estimates for milestones need to fit within that limit to be achievable and realistic.

Story point estimates are made on each issue, often through consultation with other team members. Care should be taken to avoid adding too much work to a given sprint, and the issue estimates are a good tool to gauge how conservative to be.

Some areas of the Releng code are easier to deal with than others. If the issues or epics involve modifying code in a service that is less well-known or difficult to test (e.g. auth), story point estimates should be higher by default to recognize the need for closer inspection on review.

### Choosing the next sprint
As we near the end of the current sprint, the milestone for the next sprint is often obvious based on organizational needs or follow-on work that builds on the current sprint. If there are multiple milestones possible, they should all be added to the roadmap. This helps keep customers and external parties informed.

If multiple future sprints are ready and there are no other factors to aid decision, the _Scrum master_ will decide which sprint will come next.

### Workspace configuration
TBD

### Starting the sprint
At the start of the sprint, the _Scrum master_ will update Jira to create a sprint with the sprint Epics. The _Product owner_ and _Scrum master_ will decide how and when they want to meet to review sprint progress, possibly leveraging an existing 1x1 if one exists.

We will hold a kick-off meeting where the _Product owner_ will provide context enough for people to get started and assist developers in choosing their first issue to work on. The _Scrum master_ will remind everyone of any process changes being adopted for the new sprint. Work begins.

### During the sprint
The team will hold daily stand-up meetings for the duration of the sprint. Our daily stand-ups take place in Slack asynchronously at the start of our day in Matrix, except on Tuesdays when we present our stand-up status as the first agenda item of our weekly team meeting. Whether delivered in person on via Slack, the format of the update is the same:
* DONE: work that has been completed
* TODO: work that is coming up next
* BLOCKERS: what is preventing you from getting the work done
* INTERRUPTS: what is delaying you from getting the work done

The _Product owner_ is paying attention to these updates to make sure that the most important things are being worked on and are being picked up next.

The _Scrum master_ is paying attention to these updates to make sure that blockers are highlighted and interrupts are kept to a minimum.

Once a week, the _Product owner_ and the _Scrum master_ will meet to assess sprint progress. Using the burndown chart, they figure out whether the sprint is still on track and can be completed within the allotted time. If necessary, the critical path can be refined to allow partial delivery of the original objective. Under extraordinary circumstances, they can opt to end the current sprint.

### Ending the sprint
As the sprint draws to a close the _Scrum master_ with schedule two meetings for a Review and a Retrospective. These meetings are usually scheduled back-to-back for convenience.

In the Review meeting, the _Product owner_ will lead the discussion. The focus will we be on the content of the sprint and the outcomes achieved. Feedback on the sprint content will also be collected. At the end of the Review meeting, the team will triage any outstanding issues from the sprint. The _Product owner_ will engage with developers who still have work marked as **In Progress** to figure out how and when to wrap-up that work during the _[Time between sprints](#time-between-sprints)_.  All issues that have not been started will be moved back into the **Product Backlog**.

In the Retrospective meeting, the _Scrum master_ will lead the discussion. The focus will be on the sprint process itself in an attempt to uncover grey areas and process improvements. If the team agrees to adopt a particular process change, it should be clearly marked in the meeting notes with an **ACTION** label and the person responsible for that action, if appropriate.

Notes for both meetings should be taken using the templates provided:

* sprints/
  * templates/
    * [sprint-retrospective.md](./sprints/templates/sprint-retrospective.md)
    * [sprint-review.md](./sprints/templates/sprint-review.md)

As process changes are adopted, [this document](./README.md) should be updated to reflect the new process.

### Time between sprints
We allow ourselves *one week* between sprints. This buffer allows us to analyze the previous sprint without the pressure of immediately jumping into something new. Pragmatically speaking, it also gives us the time to finish off sprint items that may still require deployment, to address unanticipated fallout from the previous sprint, and to deal with the backlog of small, timely requests that may have accumulated during the sprint.
