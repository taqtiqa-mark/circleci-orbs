# circleci-orbs
Repository holding CircleCI Orb files for the Taqtiqa namespace.

## Build Process

```
export ORB=kitchen
export ORMYML=${ORB}-orb.yml
circleci orb publish validate ${ORMYML}
circleci orb publish increment  ${ORMYML} taqtiqa/ ${ORM} major | minor |patch
```