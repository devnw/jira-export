# jira-export

[![Build Status](https://api.travis-ci.org/nortonlifelock/jira-export.svg?branch=master)](https://travis-ci.org/nortonlifelock/jira-export)
[![Go Report Card](https://goreportcard.com/badge/github.com/nortonlifelock/jira-export)](https://goreportcard.com/report/github.com/nortonlifelock/jira-export)
[![GoDoc](https://godoc.org/github.com/nortonlifelock/jira-export?status.svg)](https://godoc.org/github.com/nortonlifelock/jira-export)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

jira-export

Example Call: jira-export -url https://myjira.com -user tsmith

The Tool will request your password for the JIRA account, then ask for the JQL you wish to export. 

**NOTE: YOU MUST USE ORDER BY ON YOUR JQL QUERY. IT IS BEST TO ORDER BY CREATED DATE ASCENDING. THE REASON FOR THIS IS THAT OTHERWISE YOUR FILE WILL CONTAIN DUPLICATES THAT OVERWRITE OTHER TICKETS.**

EXAMPLE JQL: project = Aegis and status = Resolved-Remediated ORDER BY created ASC

Output Format:

KEY	| SUMMARY	| ASSIGNMENTGROUP	| STATUS	| METHODOFDISCOVERY	| ORG	| CREATED	| ALERTDATE	| DUE	| RESOLUTIONDATE	| PRIORITY	| CVSS	| CERF	| PORTS	| OS	| HOSTNAME	| IPADDRESS	| VULNERABILITY	| VULNERABILITYID	| OPERATINGSYSTEM	| SOLUTION