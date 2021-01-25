---
title: Run Your Own IG Site
---

# Run Your Own IG Site
---
---

## Host IG on GitHub and deploy with Travis
---

### Clone the repository
---

In order to develop the implementation guide, do the following steps:

- Clone the repository [https://github.com/HealthSamurai/ig-ae](https://github.com/HealthSamurai/ig-ae)

```git clone https://github.com/HealthSamurai/ig-ae.git```

- browse to the ig-ae folder

```cd ig-ae```

### Create your repository on GitHub
---

- Put the project to your GitHub repository
- Add new origin
- Push the project to your repository


### Setup configuration
---

- Add a personal access token in [your GitHub account](https://github.com/settings/tokens)
- See instructions [Creating a personal access token
](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token)
- In your repository/Settings, go to the GitHub Pages section
- Select gh-pages branch and /(root) folder
- Click Save
- Edit the `.travis.yml` file: change the "/ig-ae" to the name of your project on GitHub in the `- java -jar "./igpop/target/igpop.jar" build "/ig-ae"` line
- Edit the `ig.yaml` file:
id: hl7.fhir.ae - set the name of your project and your FHIR IG Package
title: AstraZeneca FHIR IG - this will be the main title of your IG site
url: https://healthsamurai.github.io/ig-ae - change this to your GHPages site domain. This value will be used to form your conformance resources canonical URLs
description: AstraZeneca Adverse Event Implementation Guide - this will be your IG description
fhir: 4.0.0 - remain this unchanged


### Deploy with Travis
---

- Log in to your [Travis-CI](https://travis-ci.com/) account
- Connect it to your IG project
[To get started with Travis CI using GitHub](https://docs.travis-ci.com/user/tutorial/#to-get-started-with-travis-ci-using-github)
- Add your personal access token to the Travis account with the `GITHUB_TOKEN` name
[Defining Variables in Repository Settings](https://docs.travis-ci.com/user/environment-variables#defining-variables-in-repository-settings)
- [GitHub Pages Deployment](https://docs.travis-ci.com/user/deployment/pages/)









