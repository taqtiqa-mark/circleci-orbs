# circleci-orbs
Repository holding CircleCI Orb files for the Taqtiqa namespace.

## Build Process

```
export ORB=kitchen
export ORBYML=${ORB}-orb.yml
circleci orb validate ${ORBYML}
circleci orb publish increment  ${ORBYML} taqtiqa/ ${ORB} major | minor |patch
```