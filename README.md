# Purpose 

Collect the [orbs](https://github.com/CircleCI-Public/circleci-orbs#what-are-orbs) that are used to test [istio-workspace](https://github.com/Maistra/istio-workspace/) project.

## Instruction

### Prerequisites

- [Install](https://github.com/CircleCI-Public/circleci-cli/blob/master/README.md) the CircleCI CLI
- [Obtain a token](https://circleci.com/account/api) from CircleCI dashboard

### Register a new orb with CircleCI

```shell
 circleci orb create Maistra/ike --token=xxxxx
```

###  Validate an orb

```shell
circleci orb validate ike/orb.yml
```

### Publish an orb

To publish a dev version of an orb execute:

```shell
circleci orb publish ike/orb.yml Maistra/ike@dev:master --token=xxxxx
```

To publish a prod version of an orb execute:

```shell
circleci orb publish ike/orb.yml Maistra/ike@0.1.0 --token=xxxxx
```
