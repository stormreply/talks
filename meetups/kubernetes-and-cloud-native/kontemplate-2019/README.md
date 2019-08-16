[Max Körbächer](https://github.com/mkorbi) gave this short talk at the [Munich Kubernetes Meetup](https://www.meetup.com/de-DE/Munchen-Kubernetes-Meetup/events/263419347/)

The slides will be soon available at our Website.

# Kontemplate
[Kontemplate](https://github.com/tazjin/kontemplate) is a CLI tool for resource templating for Kubernetes. In this talk I want to give a fast overview of the functionality and have a discussions with the audience about their opinion to the shown tool and for example help or RedHat operator framework.

## Show Cases
This repo containes for folders with different smal use cases.
# One
Show simple replacement/interpolation of some variables.
# Two
This example shows that you can use multiple folders, also with hirachy. 
# Three
This example shows that you can use different Kubernetes context, make the dev-values run localy while the prod values are pushed to a remote K8s.
# Four
The last show case should give an idea how the GO templating engine capabilities can be used for more complex interpolations, like UPPERCASE everything, repeat something or do a "IF" statement.

## Main commands
#### shows the rendered yaml 
kontemplate template prod-values.yaml -i app

#### do a dry run and see if it pass the kubectl
kontemplate apply prod-values.yaml --dry-run

#### apply to K8s
kontemplate apply prod-values.yaml




































simple use case, dev prod, updates via apply
context