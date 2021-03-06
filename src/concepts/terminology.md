# Terminology

* **Analyst**: Someone performing analysis.
  This is more general than **data scientist**.
* **Ping**: A message sent to our telemetry servers. Most commonly, a ping comes from Firefox and contains information on browser state, user actions, etc.
([more details](https://firefox-source-docs.mozilla.org/toolkit/components/telemetry/telemetry/data/common-ping.html)), but can also come from other Mozilla products or services
* **Dataset**: A set of data, includes ping data, derived datasets, etc. Can also refer more specifically to a [BigQuery dataset](https://cloud.google.com/bigquery/docs/datasets-intro) which is a container for tables.
* **Derived Dataset**: A processed dataset, such as `main_summary` or the
  `clients_daily` dataset
* **Session**: The time from when a Firefox browser starts until it shuts down
* **Subsession**: `Sessions` are split into `subsessions` when a 24 hour threshold is crossed or an environment change occurs
([more details](https://firefox-source-docs.mozilla.org/toolkit/components/telemetry/telemetry/concepts/sessions.html?highlight=subsession))
