---
name: Bug Report
description: Is something not working as it should? Any error messages in the logs? Something is doing strange things?
title: ""
labels: ["bug"]
body:
  - type: dropdown
    id: version
    attributes:
      label: OSISM release version
      description: What version of OSISM are you running?
      options:
        - latest
        - 7.0.4
        - 7.0.3
        - 7.0.2
        - 7.0.1
        - 7.0.0
        - 6.0.2
        - 6.0.1
        - 6.0.0
        - Some older version
      default: 0
    validations:
      required: true
  - type: textarea
    id: problem
    attributes:
      label: What's the problem?
      description: Try to describe the problem as best you can. The more details and logs we have, the better.
      value: ""
    validations:
      required: true
  - type: textarea
    id: report
    attributes:
      label: References to existing reports
      description: Sometimes you have already found the problem elsewhere (mailing list, Launchpad, Github, RedHat Bugtracker, ...)? Feel free to share the links directly here.
      value: ""
    validations:
      required: false
  - type: dropdown
    id: severity
    attributes:
      label: Severity
      description: How do you rate the severity? (A high severity initially has nothing to do with faster processing. This is only a hint for us.)
      options:
        - no choice
        - low
        - medium
        - high
      default: 0
    validations:
      required: false
  - type: dropdown
    id: urgency
    attributes:
      label: Urgency
      description: How do you rate the urgency? (A high urgency initially has nothing to do with faster processing. This is only a hint for us.)
      options:
        - no choice
        - low
        - medium
        - high
      default: 0
    validations:
      required: false
