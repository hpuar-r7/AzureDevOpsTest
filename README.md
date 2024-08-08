# Environment Variables and Secrets

The pipelines in this Repo use a number of environment variables and secrets to ensure consistency and expected behavior.

These can be set while configuring the pipeline within Azure Devops at the Review stage, or alternatively set and updated after the pipelines creation

---
## Environment Variables and Secrets used:
1. AWS_ACCESS_KEY_ID & AWS_SECRET_ACCESS_KEY
- API Key credentials of an AWS User - enabling the pipeline to interact with AWS ECR for running mimics in docker
2. BASE_URL & API_KEY
- The ICS environment to save scans to and a corresponding API Key to enable interaction without authentication
- Can be found through ICS > Settings Icon > System Administrator > System > Base URL
3. IAC_TEMPLATE_DIR_PATH
- The relative directory path from the root where IaC Templates are defined
4. Public Rapid7 ECR gallery for Mimics
- https://gallery.ecr.aws/rapid7-insightcloudsec/ics/mimics
