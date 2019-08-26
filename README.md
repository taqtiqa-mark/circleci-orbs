# circleci-orbs

Repository holding CircleCI Orb files for the Taqtiqa LLC.

## Build Process


```
export ORB=commands
export ORBYML=${ORB}-orb.yml
circleci orb validate ${ORBYML}
circleci orb publish increment  ${ORBYML} taqtiqa/${ORB} patch | minor | major
```

or

```
export ORB=kitchen
export ORBYML=${ORB}-orb.yml
circleci orb validate ${ORBYML}
circleci orb publish increment  ${ORBYML} taqtiqa/ ${ORB} patch | minor | major
```