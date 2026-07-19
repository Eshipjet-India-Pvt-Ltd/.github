# QA and Tester Sign-Off

Every production-impacting EShipJet change should receive QA validation before release.

The purpose of tester sign-off is to confirm that the right change was tested in the right environment with enough evidence for engineering, release, and support teams to trust the result.

## Required Sign-Off Template

```md
## Tester Sign-Off

Project:
Repository:
Branch:
Environment: Dev / Demo / QAS / Customer / Production
Build Version:
Ticket or Requirement:
Tester Name:
Test Date:

### Scope Tested

- [ ] Functional requirement verified
- [ ] Regression areas checked
- [ ] UI behavior verified
- [ ] API behavior verified
- [ ] Carrier workflow verified
- [ ] Rate workflow verified
- [ ] Ship workflow verified
- [ ] Void workflow verified
- [ ] Tracking workflow verified
- [ ] Label output verified
- [ ] Document output verified
- [ ] POD behavior verified
- [ ] Printer workflow verified
- [ ] Customer-specific rules verified
- [ ] Role or permission behavior verified
- [ ] Error handling verified

### Evidence

- Shipment number:
- Carrier:
- Customer:
- API endpoint or workflow:
- Screenshot or recording:
- Logs or trace reference:

### Test Result

- [ ] Passed
- [ ] Passed with notes
- [ ] Failed
- [ ] Blocked

### Notes

Add observations, limitations, failed cases, screenshots, shipment numbers, carrier responses, or pending items here.

### Sign-Off

Approved by:
Date:
```

## Tester Responsibilities

QA should verify:

- The assigned issue or requirement is fixed
- The expected environment was used
- The correct customer configuration was selected
- Regression areas were checked
- Carrier-specific workflows were tested where applicable
- Shipment, label, document, tracking, POD, and printer workflows were validated where applicable
- Any known limitation is documented before release

## Evidence Expectations

For shipping workflow changes, include one or more:

- Shipment number
- Carrier response
- Rate response
- Label output
- Tracking response
- POD or document output
- API request and response reference
- Screenshot or screen recording
- Server log reference

## Release Rule

A production-impacting change should not move to Production unless one of the following is true:

- QA has approved the change
- The release owner has documented an emergency approval
- The change is a rollback to a previously validated version

