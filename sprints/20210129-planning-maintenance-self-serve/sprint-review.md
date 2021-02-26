# Sprint Review - Planning, maintenance, and self-serve, January 11, 2021 - January 29, 2021

At the beginning of 2021, our team headcount decreased. With two previous iterations completed,
the third was aimed at planning, maintaining and improving our systems self-serve.

# Details
**Product Owner**:
- geckoview/android-components cleanup: aki
- automate mac signer maintenance: bhearsum
- password rotations:
- pushhealth: sclements
- interruptduty:
- greening-up tests: jmaher
- releng 2021 planning:
**Scrum Master**: unassigned

## Goal

Yet again we had a couple of good epics to tackle during Sprint 3. With Cam leaving,
we aimed to cover TreeHerder cross-training. Joel's [self-serve test configuration](https://firefox-source-docs.mozilla.org/testing/ci-configs/index.html)
initiative had been published and work was needed in order to implement the documented process.
Moreover, we aimed at improving our XPI-signing to reduce the KTLO and to cross-train.
Given that it was the first sprint of 2021, we targeted to do a bit of planning as well,
in order to iron things out for the roadmap.
PushHealth work was aimed as being a continuation of the previous sprint to wrap-things up,
while for automating Mac signer we wanted to take some iterative steps towards improving it.

### Epics
1. [Support and release GeckoView and Android-Components through Shipit](https://jira.mozilla.com/browse/RELENG-11)
2. [Automate Mac Signer Maintenance](https://jira.mozilla.com/browse/RELENG-22)
3. [Password Rotations & Sharing](https://jira.mozilla.com/browse/RELENG-10)
4. [Push Health UX Rework](https://jira.mozilla.com/browse/RELENG-41)
5. [Interruptduty](https://jira.mozilla.com/browse/RELENG-159)
6. [Requirements needed prior to Greening up Tests](https://jira.mozilla.com/browse/RELENG-206)
7. [Releng 2021 H1 Planning](https://jira.mozilla.com/browse/RELENG-211)

## Outcomes

GeckoView/Android-Components cleanup was mainly done as this was work carried over from Sprint 2 in order to make room for relbot and other non-releng automation.

Automate Mac Signer was largely done as a large chunk of automating configuration deployments has beed added.

Password rotation didn't get momentum, though we managed to rotate a few TreeHerder related ones.

PushHealth was largely completed with a good cross-training as well.

Interruptduty was quite busy given 85.0 release, a few dot releases for Mozilla VPN and Firefox Lite.

Greening up tests went smooth with most items completed on time.

The addons-pipeline, system addons in balrog, and mobile planning stories went very well, and the timing of doing these in sprint 3 meshed well with our planning cycle.The roadmap seemed like a shared team task that went fairly well.


## Feedback

A good side-effect of the planning phase was the planning around the releng-for-Mozilla proposal.
