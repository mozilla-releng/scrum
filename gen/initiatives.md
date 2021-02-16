# Initiatives

An _initiative_ is a collection of one or more milestones that, taken together, address one or more themes. Initiatives map to major projects that the Releng team would like to accomplish, and can be either new functionality or substantial reworks of existing functionality. Depending on the project area, an initiative can be a thin wrapper around a single milestone if that milestone is high value and self-contained.

The following are the current initiatives:

* [Keep the Lights On](#ktlo)
* [Integrate Geckoview and Android-Components in the Fenix pipeline on Shipit](#geckoview-android-components-shipit)
* [Implement Android v3 signatures and sign Fenix with them](#fenix-v3-signatures)
* [Automate shipping system addons through Balrog](#system-addons-balrog)
* [Work with the Addons team to formalize the Addons Pipeline](#formalize-addons-pipeline)
* [Automate Mac Signer Maintenance](#automate-mac-signer-maintenance)
* [Apple Silicon Support](#apple-silicon-support)
* [Push Health UX Rework](#push-health-ux-rework)
* [Password Rotations and Sharing](#password-rotations)
* [Develop Releng for Mozilla Proposal](#releng-for-mozilla-proposal)
* [Standardize Python Dependency Pinning in Gecko](#standardize-gecko-python)
* [Support Mozilla China Fenix](#mozilla-china-fenix)
* [Support tests in external contributor PRs in Android-Components](#android-components-contributor-prs)
* [Migrate Windows 10 from AWS to Azure](#migrate-windows-10-aws-to-azure)
* [Migrate from MDC2](#migrate-from-mdc2)
* [Bitbar contract renewal](#bitbar-contract-renewal)
* [Treeherder - move to CloudOps dockerflow](#treeherder-cloudops)
* [Treeherder - sheriff improvement fixes/requests](#treeherder-sheriff-requests)
* [Intermittents: quickly move repeatable failures to a quarantine job](#quarantine-intermittents)
* [EOL Firefox Lite](#firefox-lite-eol)
* [Automate Fenix Betas](#automate-fenix-betas)
* [Modernizing OS/Hardware for CI tests](#modernizing-test-platforms)
* [Developer Productivity](#developer-productivity)
* [Treeherder: Improve login experience](#treeherder-login-experience)
* [Finish Python 3 migration](#python-3-migration)
* [Make Firefox Snap the default format on Ubuntu](#firefox-snap-default)
* [Improve mobile release and CI task robustness](#mobile-task-robustness)
* [Support Focus releases through Shipit](#focus-shipit)
* [Add support for Linux ARM64 in the CI](#linux-arm64-ci)
* [TreeHerder Failure Classification](#treeherder-failure-classification)
* [Treeherder - Identify bad machines](#treeherder-bad-machines)
* [Work with l10n team to deprecate l10n repacks](#deprecate-l10n-repacks)
* [archive.mozilla.org cleanup](#archive-cleanup)
* [reduce taskgraph learning curve](#taskgraph-learning-curve)
* [Valuing Bug Sources](#valuing-bug-sources)
* [Team view of riskiness of pushes](#push-riskiness)
* [Drive desktop Firefox Nightly automation through shipit](#firefox-nightly-shipit)
* [Speed up update verify](#speed-up-update-verify)
* [Productionize or EOL ActiveData](#activedata-eol)
* [Treeherder: Maintenance/Backlog](#treeherder-maintenance)
* [Fully automate mergeduty](#automate-mergeduty)
* [Binary Transparency](#binary-transparency)
* [Upload Fenix to places where Fennec used to live](#upload-fenix-to-fennec-locations)
* [Migrate win10 tests from Datacenter to Azure](#migrate-windows-10-datacenter-to-azure)
* [Reduce wasted compute and idle time in our CI infrastructure](#task-efficiencies)
* [Right-size cloud instances](#right-size-instances)
* [Test Scheduling improvements](#test-scheduling)
* [Implement a dark mode theme in Treeherder](#treeherder-dark-mode)

To update this information, edit `data/initiatives.yml` and run `generate.py`.

## ktlo
*Keep the Lights On*

Ensure all RelEng systems are working in order to keep our products pipeline running.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20ktlo)

*Addresses Themes:*

* [Workflow](./themes.md#workflow)
* [Team Operations](./themes.md#operations)


## geckoview-android-components-shipit
*Integrate Geckoview and Android-Components in the Fenix pipeline on Shipit*

Automate GeckoView and Android-Components releases like Fenix, reducing cross-team interactions and friction.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20geckoview-android-components-shipit)

*Addresses Themes:*

* [Support user growth in Mozilla products](./themes.md#user-growth)
* [Workflow](./themes.md#workflow)


## fenix-v3-signatures
*Implement Android v3 signatures and sign Fenix with them*

We should sign Fenix with both v1 and v3 signatures so that we support legacy versions of Android while covering ourselves in case of a key leakage.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20fenix-v3-signatures)

*Addresses Themes:*

* [Workflow](./themes.md#workflow)
* [Security](./themes.md#security)


## system-addons-balrog
*Automate shipping system addons through Balrog*

Document, automate, and run periodic tests to make sure we are ready to ship system addons to all versions of Firefox through automation.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20system-addons-balrog)

*Addresses Themes:*

* [Workflow](./themes.md#workflow)
* [Security](./themes.md#security)


## formalize-addons-pipeline
*Work with the Addons team to formalize the Addons Pipeline*

Clarify and streamline the rules and process of the addons pipeline.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20formalize-addons-pipeline)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)


## automate-mac-signer-maintenance
*Automate Mac Signer Maintenance*

End goal of rolling out changes to the mac signers via ronin-puppet commit, reducing ssh and manual maintenance to zero.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20automate-mac-signer-maintenance)

*Addresses Themes:*

* [Team Operations](./themes.md#operations)
* [Security](./themes.md#security)


## apple-silicon-support
*Apple Silicon Support*

Determine what is needed to support Apple Silicon build signing and testing, and the timeframe it’s needed in.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20apple-silicon-support)

*Addresses Themes:*

* [Support user growth in Mozilla products](./themes.md#user-growth)
* [Workflow](./themes.md#workflow)


## push-health-ux-rework
*Push Health UX Rework*

Give developers a simple view of what failures seen in CI need their attention.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20push-health-ux-rework)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)


## password-rotations
*Password Rotations and Sharing*

Rotate secrets and populate the new secrets store.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20password-rotations)

*Addresses Theme:*

* [Security](./themes.md#security)


## releng-for-mozilla-proposal
*Develop Releng for Mozilla Proposal*

Create a proposal to also help non-Gecko teams at Mozilla with their release pipelines.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20releng-for-mozilla-proposal)

*Addresses Themes:*

* [Workflow](./themes.md#workflow)
* [Security](./themes.md#security)
* [Support user growth in Mozilla products](./themes.md#user-growth)


## standardize-gecko-python
*Standardize Python Dependency Pinning in Gecko*

Work with the Build team to standardize how we pin and install dependencies across Gecko, including developer virtualenvs, automated builds, and automated tests.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20standardize-gecko-python)

*Addresses Themes:*

* [Security](./themes.md#security)
* [Workflow](./themes.md#workflow)


## mozilla-china-fenix
*Support Mozilla China Fenix*

Automate a Mozilla China variant of Fenix in the official Fenix repo, at the same cadence as other Fenix releases.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20mozilla-china-fenix)

*Addresses Themes:*

* [Security](./themes.md#security)
* [Workflow](./themes.md#workflow)


## android-components-contributor-prs
*Support tests in external contributor PRs in Android-Components*

Potentially install and support Bors for automated tests in PRs without exposing secrets to the internet.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20android-components-contributor-prs)

*Addresses Themes:*

* [Security](./themes.md#security)
* [Workflow](./themes.md#workflow)


## migrate-windows-10-aws-to-azure
*Migrate Windows 10 from AWS to Azure*

Migrate our Windows 10 tasks from AWS to Azure.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20migrate-windows-10-aws-to-azure)

*Addresses Themes:*

* [Team Operations](./themes.md#operations)
* [Support cost reduction](./themes.md#cost-reduction)


## migrate-from-mdc2
*Migrate from MDC2*

Support the migration out of MDC2.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20migrate-from-mdc2)

*Addresses Themes:*

* [Team Operations](./themes.md#operations)
* [Support cost reduction](./themes.md#cost-reduction)


## bitbar-contract-renewal
*Bitbar contract renewal*

Contract expires mid-April. We need a solution for android/fenix/laptop perf testing and to plan capacity in a budget-friendly way. With some minimum efforts, we could save ~$100K

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20bitbar-contract-renewal)

*Addresses Themes:*

* [Team Operations](./themes.md#operations)
* [Support cost reduction](./themes.md#cost-reduction)


## treeherder-cloudops
*Treeherder - move to CloudOps dockerflow*

Mitigate risk of only having a small handful of people who could respond to emergencies. Also brings consistency across rest of the RelEng major systems that are already in CloudOps's hands.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20treeherder-cloudops)

*Addresses Themes:*

* [Team Operations](./themes.md#operations)
* [Workflow](./themes.md#workflow)


## treeherder-sheriff-requests
*Treeherder - sheriff improvement fixes/requests*

There are fixes they've been asking for for many years that add up to lost productivity

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20treeherder-sheriff-requests)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)


## quarantine-intermittents
*Intermittents: quickly move repeatable failures to a quarantine job*

Ability to run tests in quarantine as part of new config process, desire to reduce load on code sheriffs, existing processes depend on activedata which isn't well supported anymore

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20quarantine-intermittents)

*Addresses Themes:*

* [Workflow](./themes.md#workflow)
* [Support cost reduction](./themes.md#cost-reduction)


## firefox-lite-eol
*EOL Firefox Lite*

Firefox Lite is no longer supported, but we want to create a few more releases to notify users and send them to other products. We no longer have a team creating these releases; let's help the mobile team get these releases signed and shipped.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20firefox-lite-eol)

*Addresses Theme:*

* [Team Operations](./themes.md#operations)


## automate-fenix-betas
*Automate Fenix Betas*

Fenix beta timing requires RelMan to be around in the north american evening to trigger them. We should be able to automate this relatively easily to make their lives better

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20automate-fenix-betas)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)


## modernizing-test-platforms
*Modernizing OS/Hardware for CI tests*

Keep Firefox CI OS+hardware/cloud environments relevant and investigate ways to reduce pain points.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20modernizing-test-platforms)

*Addresses Themes:*

* [Team Operations](./themes.md#operations)
* [Workflow](./themes.md#workflow)


## developer-productivity
*Developer Productivity*

Improve developer productivity by addressing bugs developers file/mention and being proactive on workflows

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20developer-productivity)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)


## treeherder-login-experience
*Treeherder: Improve login experience*

Minimize papercuts in Treeherder by increasing login TTL.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20treeherder-login-experience)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)


## python-3-migration
*Finish Python 3 migration*

Python 2 has been EOLed since the end of 2019. Pip dropped support for Python 2.7 in Jan 2021.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20python-3-migration)

*Addresses Themes:*

* [Team Operations](./themes.md#operations)
* [Security](./themes.md#security)


## firefox-snap-default
*Make Firefox Snap the default format on Ubuntu*

Make Snap the default format on Ubuntu. This will make a Mozilla build the default, rather than a distribution rebuild. There may be contracts involved.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20firefox-snap-default)

*Addresses Themes:*

* [Workflow](./themes.md#workflow)
* [Security](./themes.md#security)
* [Support user growth in Mozilla products](./themes.md#user-growth)


## mobile-task-robustness
*Improve mobile release and CI task robustness*

Intermittent failures are forcing mobile developers to rerun 100+ tasks instead of automatically rerunning; let's improve that.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20mobile-task-robustness)

*Addresses Themes:*

* [Workflow](./themes.md#workflow)
* [Team Operations](./themes.md#operations)


## focus-shipit
*Support Focus releases through Shipit*

Let's unify our mobile pipelines by supporting Focus in shipit.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20focus-shipit)

*Addresses Themes:*

* [Workflow](./themes.md#workflow)
* [Security](./themes.md#security)


## linux-arm64-ci
*Add support for Linux ARM64 in the CI*

Better ARM64 automated testing overall. M1 automatic testing will be hard at scale. Testing more on Linux will help identifying CPU specific issue for both Linux and Apple Silicon since they are very similar. Would help for mobile too since most of Android is ARM64.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20linux-arm64-ci)

*Addresses Themes:*

* [Team Operations](./themes.md#operations)
* [Workflow](./themes.md#workflow)


## treeherder-failure-classification
*TreeHerder Failure Classification*

This is a common request from sheriffs. Not having this is slowing their work and decreasing accuracy.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20treeherder-failure-classification)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)


## treeherder-bad-machines
*Treeherder - Identify bad machines*

Effort to reduce sheriff load, spending 2h/week finding patterns and investigating

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20treeherder-bad-machines)

*Addresses Themes:*

* [Workflow](./themes.md#workflow)
* [Support cost reduction](./themes.md#cost-reduction)


## deprecate-l10n-repacks
*Work with l10n team to deprecate l10n repacks*

There is momentum from the l10n team on this. This would exponentially reduce taskgraph complexity and release end-to-end times. We would reduce the number of shipping desktop binaries exponentially. Repacks are also significantly less discoverable or configurable on shared/multilingual users’ machines than langpacks could be.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20deprecate-l10n-repacks)

*Addresses Themes:*

* [Support cost reduction](./themes.md#cost-reduction)
* [Workflow](./themes.md#workflow)
* [Support user growth in Mozilla products](./themes.md#user-growth)


## archive-cleanup
*archive.mozilla.org cleanup*

Get rid of unnecessary files on archive.mozilla.org and enact new retention policies

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20archive-cleanup)

*Addresses Theme:*

* [Support cost reduction](./themes.md#cost-reduction)


## taskgraph-learning-curve
*reduce taskgraph learning curve*

Improving the tool reduces the learning curve for Releng, saves us future effort, helps with better automation and adds more self-serving capabilities for other teams that are using it.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20taskgraph-learning-curve)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)


## valuing-bug-sources
*Valuing Bug Sources*

We pay a significant amount to various sources to file new bugs. By creating a tool to show relative values of each bug filing source, we can determine whether each is worth the cost.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20valuing-bug-sources)

*Addresses Theme:*

* [Support cost reduction](./themes.md#cost-reduction)


## push-riskiness
*Team view of riskiness of pushes*

The idea is to move some of the knowledge and responsibility that is currently RelMan’s and spread it across engineering teams. Distributed responsibility should make it easier to control quality, since each team will take ownership of quality for the components they own rather than relying on a small "third-party" team to oversee everything.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20push-riskiness)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)


## firefox-nightly-shipit
*Drive desktop Firefox Nightly automation through shipit*

Unify nightly and release automation in Gecko.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20firefox-nightly-shipit)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)


## speed-up-update-verify
*Speed up update verify*

Speed up update verify.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20speed-up-update-verify)

*Addresses Themes:*

* [Support cost reduction](./themes.md#cost-reduction)
* [Workflow](./themes.md#workflow)


## activedata-eol
*Productionize or EOL ActiveData*

Productionize or EOL ActiveData.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20activedata-eol)

*Addresses Theme:*

* [Team Operations](./themes.md#operations)


## treeherder-maintenance
*Treeherder: Maintenance/Backlog*

Treeherder maintenance and backlog

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20treeherder-maintenance)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)


## automate-mergeduty
*Fully automate mergeduty*

Fully automate the rest of mergeduty.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20automate-mergeduty)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)


## binary-transparency
*Binary Transparency*

Implement Binary Transparency for Firefox updates

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20binary-transparency)

*Addresses Theme:*

* [Security](./themes.md#security)


## upload-fenix-to-fennec-locations
*Upload Fenix to places where Fennec used to live*

Backup Fenix artifacts in S3 for future + update Buildhub for automation downstream consumption. Not urgent but nice-to-have. request from the mobile team too

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20upload-fenix-to-fennec-locations)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)


## migrate-windows-10-datacenter-to-azure
*Migrate win10 tests from Datacenter to Azure*

datacenter machines are past warranty and need to be replaced in 2022, work in 2021 to capacity plan and evaluate new machines

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20migrate-windows-10-datacenter-to-azure)

*Addresses Themes:*

* [Team Operations](./themes.md#operations)
* [Support cost reduction](./themes.md#cost-reduction)


## task-efficiencies
*Reduce wasted compute and idle time in our CI infrastructure*

Reduce test frequencies, wasted time in tasks, and idle time in our CI infrastructure.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20task-efficiencies)

*Addresses Theme:*

* [Support cost reduction](./themes.md#cost-reduction)


## right-size-instances
*Right-size cloud instances*

Create system to identify tasks running on oversized instances by collecting resource usage data into our data analytics platform (BigQuery)

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20right-size-instances)

*Addresses Theme:*

* [Support cost reduction](./themes.md#cost-reduction)


## test-scheduling
*Test Scheduling improvements*

Use smarter scheduling algorithms to reduce the number of tasks we run in CI and give developers greater confidence in their try pushes.

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20test-scheduling)

*Addresses Themes:*

* [Support cost reduction](./themes.md#cost-reduction)
* [Workflow](./themes.md#workflow)


## treeherder-dark-mode
*Implement a dark mode theme in Treeherder*

Per camd, this has been a popular feature request from sheriffs for a while and he had taken a stab at it in the past but found it was too much work with competing, higher priorities (one of the challenges being the amount of custom CSS we have and keeping the contrast between various colors accessible).

[*Associated Epics*](https://jira.mozilla.com/issues/?jql=project%20%3D%20RELENG%20AND%20issuetype%20%3D%20Epic%20AND%20labels%20%3D%20treeherder-dark-mode)

*Addresses Theme:*

* [Workflow](./themes.md#workflow)

