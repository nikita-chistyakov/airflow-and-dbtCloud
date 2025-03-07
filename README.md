# Airflow_and_dbtCloud

Many organization already use Airflow to orchestrate their data workflows. dbt Cloud works great with Airflow, allowing to execute my dbt code in dbt Cloud while keeping orchestration duties with Airflow. 
This ensures the project's metadata (important for tools like dbt Explorer) is available and up-to-date, while still enabling me to use Airflow for general tasks such as:

- Scheduling other processes outside of dbt runs
- Ensuring that a dbt job kicks off before or after another process outside of dbt Cloud
- Triggering a dbt job only after another has completed

In this repository, I'm practicing how to:

- Create a working local Airflow environment
- Invoke a dbt Cloud job with Airflow
- Reuse tested and trusted Airflow code for a specific use cases

I’ll also gain a better understanding of how this will:

- Reduce the cognitive load when building and maintaining pipelines
- Avoid dependency hell (think: pip install conflicts)
- Define clearer handoff of workflows between data engineers and analytics engineers
