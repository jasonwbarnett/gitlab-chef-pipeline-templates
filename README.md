# pipeline-templates

This repo contains templates for `.gitlab-ci.yml` for publishing Chef artifacts.

You can use these in [GitLab](https://about.gitlab.com/) CI by setting you your `.gitlab-ci.yml` like so:

```yml
---
include: "https://git.dayold.pizza/kevinreedy/pipeline-templates/raw/master/cookbook.yml"
```

Note: this doesn't work with the Community Edition of GitLab
