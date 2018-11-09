# gitlab-autodevops

Templates for GitLab CI/CD and Helm chart for Kubernetes

### Template for gitlab-ci.yml

In order to use gitlab-ci.yml template use the following code:

```yaml
include: 'https://raw.githubusercontent.com/PayU/gitlab-autodevops/master/gitlab-ci-template.yml'
```

### Helm chart for Kubernetes

Chart can be fetched by:

```
helm fetch https://github.com/PayU/gitlab-autodevops/archive/master.zip
```

### CI/CD variables

| Variable | Default | Description |
| -------- | ------- | ----------- |
| **APP_HEALTH_CHECK_ENDPOINT** | ```/``` | Endpoint for Kubernetes to test node availability |

##### References

* [Auto-DevOps.gitlab-ci.yml](https://gitlab.com/gitlab-org/gitlab-ce/blob/master/lib/gitlab/ci/templates/Auto-DevOps.gitlab-ci.yml)
* [Auto-deploy-app Chart used by AutoDevOps](https://gitlab.com/charts/auto-deploy-app/tree/master)