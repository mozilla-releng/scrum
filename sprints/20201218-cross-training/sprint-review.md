# Sprint Review - Cross-Training, November 30, 2020 - December 18, 2020

After a trial run sprint 1 iteration, we decided to take multiple product owners (epic champions could be their own product owner) in the second iteration, which should also be properly tracked in JIRA.

## Details
**Product Owner**:
- mozillavpn: bhearsum
- android-components on shipit: jlorenzo
- apple silicon: jmaher
- interruptduty: mtabara
- treeherder sheriff: camd
- push health: sclements
**Scrum Master**: mtabara

## Goal

A couple of competing priories have met during our second iteration. The starting point was cross-training as the bus factor for the
mobile automation was low. Moreover, VPN 2.0 release was undergoing and had RelEng as blocking vector. Similarly Apple Silicon native
support for Firefox was targetted for Firefox 84.0 (2020-12-15).

On top of all these, we had planned to tackle some low-hanging fruits to fix papercuts in TreeHerder in order to optimize Sheriffs' workflow.
Last but not least, PushHealth was close to the finish line in order to be ready for full roll-out.

### Epics
1. [Make it possible to ship MozillaVPN 2.0](https://jira.mozilla.com/browse/RELENG-107)
2. [Support and release GeckoView and Android-Components through Shipit](https://jira.mozilla.com/browse/RELENG-11)
3. [Support automated tests on Apple Silicon](https://jira.mozilla.com/browse/RELENG-79)
4. [Interruptduty](https://jira.mozilla.com/browse/RELENG-159)
5. [Treeherder - Sheriff requests 1](https://jira.mozilla.com/browse/RELENG-31)
6. [Push Health UX Rework](https://jira.mozilla.com/browse/RELENG-41)

## Outcomes

Mozilla VPN was done, all of the things that were planned were either done or explicitly descoped. Most notable thing to note is it didn’t go well with the cross training theme because of the tight deadline.

Android-Components went well as well, with great results for cross-training as well. Rolled-out, left the old way of doing things as fallback solution. We learned more from Stefan as well from his side of automation. Timezone was a bit hectic but Aki had enough context to provide to help out.

Apple Silicon was a solo-project for Joel as there wasn't realistically room for parallelization or cross-training. Most of it got done, though not tracked in JIRA.

Interruptduty was okay, but not great. We started tracking some of the interrupts with daily comments and we managed to cross-train on releaseduty and treeherderduty. On the other hand, not everything was tracked. Lots of confusion in the end about what should be tracked as interruptduty (email, meetings, disruptive requests to derail work, etc).

Treeherder for Sheriffs was good for cross-training, went well and was completed.

PushHealth was a backburner from the beginning, went well given the amount was able to be spent on it.


## Feedback
Big win for VPN was the planning which was really well upfront, with work broken down well before sprint started.

For Android-Components, timezone was a bit hectic, reminding ourselves that's something to take into account when planning epics.

Interruptduty was good for cross-training, not great for scope as all the unknown unknown are hard to track. Maybe over time it will get better.

Consensus was that we got more focused work done with the sprint than otherwise.
