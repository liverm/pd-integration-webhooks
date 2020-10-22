# pd-integration_webhooks

A collection of JSON-formatted webhooks that send PD-CEF-formatted events.  All the JSON files are designed to send an Events V2 API payload.  To create the necessary API key please consult the following PagerDuty documentation:

* [PagerDuty Rulesets](https://support.pagerduty.com/docs/rulesets#send-events-to-a-global-ruleset)
* [PagerDuty Services and Integrations](https://support.pagerduty.com/docs/rulesets#send-events-to-a-global-ruleset)

# eggplant2pd.json

Details on how to configure a webhook for alerts in Eggplant Monitoring Insights is detailed on [Eggplant's support pages](http://docs.eggplantsoftware.com/EMI/emi-webhooks.htm).  For PagerDuty, the settings should be as follows.

REQUEST METHOD:
post

URL:
https://events.pagerduty.com/v2/enqueue

REQUEST HEADERS:
content-type: application/json
x-routing-key: <Insert Routing Key>

BODY PAYLOAD:
Copy the contents of the JSON file.
