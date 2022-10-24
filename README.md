# stanza_logging
Log to GCP Cloud Logging using Stanza agents
  
These are example config files for the Stanza logging agent.  The show a windows based host that logs powershell/eventlogs/sysmon as well as a linux based host that uses stanza as a syslog receiver and local file tailer with multiple pipeline paths, transforms, and outputs.
  
Get information on Stanza as well as the agents from here:  
https://github.com/observIQ/stanza  

## GCP Logging Service Account
You will need a service account in the GCP Project that you want to write logs into.  The service account roles that have worked for me are:

* Logs Bucket Writer
* Logs Writer

The JSON credential file will need to be saved on any system that runs the Stanza agent so that they can push events directly to GCP Cloud Logging.
