# Initiatives

An _initiative_ is a collection of one or more milestones that, taken together, address one or more themes. Initiatives map to major projects that the Taskcluster team would like to accomplish, and can be either new functionality or substantial reworks of existing functionality. Depending on the project area, an initiative can be a thin wrapper around a single milestone if that milestone is high value and self-contained.

The following are the current initiatives:

* [Keep the Lights On](#ktlo)
* [Automation Needs](#automation-needs)
* [Initiate and drive Fenix release automation through the Shipit service](#fenix-shipit)
* [Apple Silicon Support](#apple-silicon-support)
* [Test Scheduling improvements](#test-scheduling)
* [Implement Android v3 signatures and sign Fenix with them](#fenix-v3-signatures)
* [Rotate releng secrets and share with the team](#secrets-rotation)
* [Integrate Geckoview and Android-Components in the Fenix pipeline on Shipit](#geckoview-android-components-shipit)
* [Reduce wasted compute and idle time in our CI infrastructure](#task-efficiencies)
* [ActiveData Maintenance](#activedata-maintenance)
* [Right-size cloud instances](#right-size-instances)
* [Balrog Metadata Submission](#balrog-metadata)
* [Push Health UX Rework](#push-health-ux-rework)
* [Automated MozillaVPN signing](#mozillavpn-signing)
* [Specific bug fixes and feature requests for sheriffs](#treeherder-sheriff-requests)
* [Finish Python 3 migration](#python-3-migration)
* [Push Health MozCI integration](#push-health-mozci)
* [Test distribution and scheduling optimizations](#test-distribution-optimization)
* [Developer Productivity](#developer-productivity)
* [archive.mozilla.org cleanup](#archive-cleanup)
* [Improve iOS build, release, and CI pipeline](#ios-needs)

To update this information, edit `data/initiatives.yml` and run `generate.py`.

## ktlo
*Keep the Lights On*

Ensure all RelEng systems are working in order to keep our products pipeline running.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Aktlo)

*Addresses Themes:*

* [Project Maintenance](./themes.md#maintenance)
* [Team Operations](./themes.md#operations)


## automation-needs
*Automation Needs*

Keep Firefox CI OS+hardware/cloud environments relevant and investigate ways to reduce pain points.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Aautomation-needs)

*Addresses Theme:*

* [Project Maintenance](./themes.md#maintenance)


## fenix-shipit
*Initiate and drive Fenix release automation through the Shipit service*

Support Fenix in Shipit, reducing human error and time spent shepherding Fenix releases.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Afenix-shipit)

*Addresses Themes:*

* [Support user growth in Mozilla products](./themes.md#user-growth)
* [Project Maintenance](./themes.md#maintenance)


## apple-silicon-support
*Apple Silicon Support*

Determine what is needed to support Apple Silicon build signing and testing, and the timeframe it’s needed in.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Aapple-silicon-support)

*Addresses Themes:*

* [Support user growth in Mozilla products](./themes.md#user-growth)
* [Project Maintenance](./themes.md#maintenance)


## test-scheduling
*Test Scheduling improvements*

Use smarter scheduling algorithms to reduce the number of tasks we run in CI and give developers greater confidence in their try pushes.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Atest-scheduling)

*Addresses Themes:*

* [Support cost reduction](./themes.md#cost-reduction)
* [Project Maintenance](./themes.md#maintenance)


## fenix-v3-signatures
*Implement Android v3 signatures and sign Fenix with them*

We should sign Fenix with both v1 and v3 signatures so that we support legacy versions of Android while covering ourselves in case of a key leakage.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Afenix-v3-signatures)

*Addresses Theme:*

* [Project Maintenance](./themes.md#maintenance)


## secrets-rotation
*Rotate releng secrets and share with the team*

Rotate releng secrets.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Asecrets-rotation)

*Addresses Themes:*

* [Project Maintenance](./themes.md#maintenance)
* [Team Operations](./themes.md#operations)


## geckoview-android-components-shipit
*Integrate Geckoview and Android-Components in the Fenix pipeline on Shipit*

Automate GeckoView and Android-Components releases like Fenix, reducing cross-team interactions and friction.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Ageckoview-android-components-shipit)

*Addresses Themes:*

* [Support user growth in Mozilla products](./themes.md#user-growth)
* [Project Maintenance](./themes.md#maintenance)


## task-efficiencies
*Reduce wasted compute and idle time in our CI infrastructure*

Reduce test frequencies, wasted time in tasks, and idle time in our CI infrastructure.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Atask-efficiencies)

*Addresses Theme:*

* [Support cost reduction](./themes.md#cost-reduction)


## activedata-maintenance
*ActiveData Maintenance*

Keep ActiveData running, until we find alternate solutions.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Aactivedata-maintenance)

*Addresses Theme:*

* [Project Maintenance](./themes.md#maintenance)


## right-size-instances
*Right-size cloud instances*

Create system to identify tasks running on oversized instances by collecting resource usage data into our data analytics platform (BigQuery)

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Aright-size-instances)

*Addresses Theme:*

* [Support cost reduction](./themes.md#cost-reduction)


## balrog-metadata
*Balrog Metadata Submission*

Rework the Balrog admin interface to optimize how update metadata about individual locales is submitted, to increase reliability and efficiency.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Abalrog-metadata)

*Addresses Themes:*

* [Project Maintenance](./themes.md#maintenance)
* [Team Operations](./themes.md#operations)


## push-health-ux-rework
*Push Health UX Rework*

Give developers a simple view of what failures seen in CI need their attention.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Apush-health-ux-rework)

*Addresses Theme:*

* [Project Maintenance](./themes.md#maintenance)


## mozillavpn-signing
*Automated MozillaVPN signing*

Set up automated signing for MozillaVPN.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Amozillavpn-signing)

*Addresses Theme:*

* [Support user growth in Mozilla products](./themes.md#user-growth)


## treeherder-sheriff-requests
*Specific bug fixes and feature requests for sheriffs*

Improving workflows for sheriffs make them more efficient and accurate. It also makes their lives easier.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Atreeherder-sheriff-requests)

*Addresses Theme:*

* [Project Maintenance](./themes.md#maintenance)


## python-3-migration
*Finish Python 3 migration*

Python 2 has been EOLed since the end of 2019. Pip will drop support for Python 2.7 in Jan 2021.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Apython-3-migration)

*Addresses Theme:*

* [Project Maintenance](./themes.md#maintenance)


## push-health-mozci
*Push Health MozCI integration*

Improve Push Health regression detection accuracy by integrating MozCI

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Apush-health-mozci)

*Addresses Theme:*

* [Project Maintenance](./themes.md#maintenance)


## test-distribution-optimization
*Test distribution and scheduling optimizations*

Reduce overhead related to getting test files onto the test workers; stop scheduling builds for test-only changes.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Atest-distribution-optimization)

*Addresses Themes:*

* [Support cost reduction](./themes.md#cost-reduction)
* [Project Maintenance](./themes.md#maintenance)


## developer-productivity
*Developer Productivity*

Improve developer productivity by addressing bugs developers file/mention and being proactive on workflows

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Adeveloper-productivity)

*Addresses Theme:*

* [Project Maintenance](./themes.md#maintenance)


## archive-cleanup
*archive.mozilla.org cleanup*

Get rid of unnecessary files on archive.mozilla.org and enact new retention policies

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Aarchive-cleanup)

*Addresses Theme:*

* [Support cost reduction](./themes.md#cost-reduction)


## ios-needs
*Improve iOS build, release, and CI pipeline*

iOS builds & releases are more important than ever, and ensuring developers are unblocked and that releases can ship on time is very important.

[*Associated Epics*](https://github.com/taskcluster/scrum/issues?q=is%3Aissue+is%3Aopen+label%3Ainitiative%3Aios-needs)

*Addresses Theme:*

* [Support user growth in Mozilla products](./themes.md#user-growth)

