# pipeline-templates

This repo contains templates for `.gitlab-ci.yml` for publishing Chef artifacts.

## Using as a template
You can use and extend these in [GitLab](https://about.gitlab.com/) CI by setting you your `.gitlab-ci.yml` like so:

```yml
---
include: "https://git.dayold.pizza/kevinreedy/pipeline-templates/raw/master/cookbook.yml"
```

Note: this doesn't work with the Community Edition of GitLab

## Secrets
To upload your artifacts, you'll need keys. These runner configs assume there will be a knife config on disk at `/opt/chef-secrets/chef/.chef/knife.rb` and an InSpec config at `/opt/chef-secrets/inspec/.inspec/compliance/config.json`. You can change or override these as necessary.
