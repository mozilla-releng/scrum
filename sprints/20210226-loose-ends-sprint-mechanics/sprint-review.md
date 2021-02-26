# Sprint Review - Loose ends and sprint mechanics, February 08, 2021 - February 26, 2021

Sprint 4 added some momentum to our sprint working model. Some seeds we have planted
in sprin3 were pending sprouting so we dedicated the time for this sprint to
close some loose ends and put some things behind us in the Done sections.

# Details
**Product Owner**:
- automate mac signer maintenance: bhearsum
- activedata eol: mtabara
- password rotations:
- pushhealth: sclements
- mozillavpn automated signing: bhearsum
- interruptduty:
- osx r8 migration: jmaher
- bitbar capacity planning: jmaher
- mdc1: jmaher
- system-addons balrog: aki
- releng for mozilla: bhearsum
- releng hiring: mtabara
- firefox mr1: mtabara
**Scrum Master**: unassigned

## Goal

While working on the 2021 releng roadmap, for sprint 4 we buckled together a couple
of loose ends items to help us close some chapters. First, we wanted to make some
more progress on automating mac signer maintanence to help us streamline our automation
and deployment process to make it consistent. ActiveData has been broken for quite some time
now and our motivation was to take a stab at identifying all its upstream pushers and downstream consumers.
Password rotation is a regular routine undertaking while for PushHealth we aimed at
wrapping things up and make it presentation-ready for the larger audience. Mozilla VPN signing
has been working smooth for us to serve the dot releases, but there were still some hiccups to
streamline things.
On the automated testing side, a few tasks were mandatory: to migrate our OSX R8 workers,
to plan our capacity for Bitbar and to handle the MDC1 internal migration.
Moreover we aimed at working with the addons team to make some adjustements there, while
also wrapping up our proposal for releng-for-Mozilla.

### Epics
1. [Automate Mac Signer Maintenance](https://jira.mozilla.com/browse/RELENG-22)
2. [ActiveData EOL](https://jira.mozilla.com/browse/RELENG-12)
3. [Password Rotations & Sharing](https://jira.mozilla.com/browse/RELENG-10)
4. [Push Health UX Rework](https://jira.mozilla.com/browse/RELENG-41)
5. [Automate Signing for MozillaVPN](https://jira.mozilla.com/browse/RELENG-131)
6. [Interruptduty](https://jira.mozilla.com/browse/RELENG-159)
7. [migrate OSX perf tests from R7 minis (w/Mojave) -> R8 minis (w/Catalina)](https://jira.mozilla.com/browse/RELENG-251)
8. [bitbar capacity planning](https://jira.mozilla.com/browse/RELENG-258)
9. [datacenter migration and changes](https://jira.mozilla.com/browse/RELENG-276)
10. [addons-pipeline: support submitting system addons to balrog](https://jira.mozilla.com/browse/RELENG-291)
11. [RelEng for Mozilla Planning](https://jira.mozilla.com/browse/RELENG-335)
12. [RelEng hiring](https://jira.mozilla.com/browse/RELENG-342)
13. [Firefox MR1](https://jira.mozilla.com/browse/RELENG-347)

## Outcomes

## Feedback
