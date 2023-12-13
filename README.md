### Using kubectl-ai to create YAML manifests

**Installation kubectl-ai**

```console
brew tap sozercan/kubectl-ai https://github.com/sozercan/kubectl-ai
brew install kubectl-ai
```

Create an API key at https://platform.openai.com/account/api-keys

```console
export OPENAI_API_KEY=<your OpenAI key>
export OPENAI_DEPLOYMENT_NAME=<your OpenAI deployment/model name. defaults to "gpt-3.5-turbo-0613">
```


| Name                      | PROMPT                                                   | DESCRIPTION                                                                                   | EXAMPLE                              |
|---------------------------|----------------------------------------------------------|-----------------------------------------------------------------------------------------------|--------------------------------------|
| app.yaml                  | Create a configuration manifest for an nginx application. | A Kubernetes manifest for setting up an nginx application, detailing deployment and service specifications. | [app.yaml example](/yaml/app.yaml) |
| app-livenessProbe.yaml    | Create a liveness probe manifest specifically for an nginx application. | Kubernetes manifest for a Pod resource, includes a configuration for a liveness probe targeted at an nginx app. | [app-livenessProbe.yaml example](/yaml/app-livenessProbe.yaml) |
| app-readinessProbe.yaml   | Create a readiness probe setup for an nginx application. | Kubernetes manifest for a Pod resource, includes a configuration for a readiness probe for an nginx application. | [app-readinessProbe.yaml example](/yaml/app-readinessProbe.yaml) |
| app-volumeMounts.yaml     | Create a volume mounts configuration for an nginx application. | Kubernetes manifest detailing the process of mounting storage volumes within an nginx application pod. | [app-volumeMounts.yaml example](/yaml/app-volumeMounts.yaml) |
| app-cronjob.yaml          | Create a cron job manifest tailored to an nginx application. | A manifest for creating a cron job in Kubernetes, specifically designed to run recurring tasks in an nginx application. | [app-cronjob.yaml example](/yaml/app-cronjob.yaml) |
| app-job.yaml              | Create a job manifest suitable for an nginx application. | Kubernetes manifest for creating a Job resource, designed to execute batch jobs in an nginx application environment. | [app-job.yaml example](/yaml/app-job.yaml) |
| app-multicontainer.yaml   | Create a multi-container pods manifest optimized for nginx. | Kubernetes manifest for configuring multi-container pods, specifically designed to efficiently run an nginx application. | [app-multicontainer.yaml example](/yaml/app-multicontainer.yaml) |
| app-resources.yaml        | Create a resource usage specification for an nginx application. | A manifest outlining resource allocation and limitations for an nginx application in a Kubernetes environment. | [app-resources.yaml example](/yaml/app-resources.yaml) |
| app-secret-env.yaml       | Create a manifest for integrating Secrets as environment variables. | Kubernetes manifest to set up environment variables sourced from Secrets, enhancing security in application configuration. | [app-secret-env.yaml example](/yaml/app-secret-env.yaml) |
