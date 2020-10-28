# pd-integration-webhooks

A collection of JSON-formatted webhooks that send PD-CEF-formatted events.  All the JSON files are designed to send an Events V2 API payload.  To create the necessary Events API routing key please consult the following PagerDuty documentation:

* [PagerDuty Rulesets](https://support.pagerduty.com/docs/rulesets#send-events-to-a-global-ruleset)
* [PagerDuty Services and Integrations](https://support.pagerduty.com/docs/services-and-integrations#create-a-generic-events-api-integration)

# eggplant2pd.json

Details on how to configure a webhook for alerts in Eggplant Monitoring Insights are detailed on [Eggplant's support pages](http://docs.eggplantsoftware.com/EMI/emi-webhooks.htm).  For PagerDuty, the settings should be as follows.

REQUEST METHOD:
post

URL:
https://events.pagerduty.com/v2/enqueue

REQUEST HEADERS:
content-type: application/json

BODY PAYLOAD:
Copy the contents of the JSON file.
