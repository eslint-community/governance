# ESLint-Community Governance

## Core Team

The Core Team are the curators and stewards of the ESLint-Community project . Their key
responsibility is to evaluate new projects that are proposed to join `@eslint-community`
and to help out in offering a base level maintenance for all primary projects within
the organization.

The Core Team should have occasional meetings to discuss the project, with meeting minutes
being added to [eslint-community/governance](https://github.com/eslint-community/governance).

The Core Team are together with the ESLint TSC the organization owners and the only ones
with `admin` access to repositories within the organization.

The Core Team are the only members of the `@eslint-community/core-team` team.

The Core Team and ESLint TSC have a shared `#community-team` chat room, in the ESLint
Discord, to communicate with one another.

## ESLint TSC

The ESLint TSC are the ultimate caretakers of the ESLint-Community, appoints the Core
Team and holds the ownership of the `eslint-community-bot` npm account that owns all
the ESLint-Community npm modules.

The Core Team are together with the ESLint TSC the organization owners and only ones
with `admin` access to repositories within the organization.

The ESLint TSC are the only members of the `@eslint-community/eslint-tsc` team.

The Core Team and ESLint TSC have a shared `#community-team` chat room, in the ESLint
Discord, to communicate with one another.

## Collaborators

Collaborators maintain the projects of the ESLint-Community organization.

Collaborators are added on a project by project basis by adding them to a team of
the same name as its main project repository, eg. `@eslint-community/eslint-plugin`.

A project team is given `write` level access to its repositories.

If multiple repositores are needed by the same project they should all be added to
the project team.

Both Collaborators and non-Collaborators may propose changes to the source code
of the projects of the organization. The mechanism to propose such a change is a
GitHub pull request. Collaborators review and merge (_land_) pull requests
following the [CONTRIBUTING](CONTRIBUTING.md) guidelines.

Collaborators can communicate in private with the Core Team [on GitHub](https://github.com/eslint-community/collaborators/discussions).

### Collaborator activities

* Helping users and novice contributors
* Contributing code and documentation changes that improve the project
* Reviewing and commenting on issues and pull requests
* Merging pull requests
* Release plugins

The Core Team can remove inactive Collaborators or provide them with
_Past Collaborators_ status. Past Collaborators may request that the Core
Team restore them to active status.

## Projects

There are two kinds of projects in ESLint Community: Primary and auxiliary projects.

Primary projects are maintained by Core Team in collaboration with project Collaborators
and will be ensured to be kept up to date at a best effort pace by the Core Team.

Auxiliary projects are maintained by its project Collaborators and is kept up to date at
whatever pace those Collaborators chose. The Core Team merely fascilitates nominations
of new Collaborators to such projects, ensuring there's a path to keep it maintained,
without making any promises.

All project npm modules should be owned (and solely owned) by the `eslint-community-bot`
user on npm. If the npm modules are owned by an existing organisation and using its prefix,
then the `eslint-community-bot` should become the sole owner of that organisation.

Additional assets such as domain names, web sites etc should also be in control of the
Core Team and/or the ESLint TSC.

If possible, a project should always be transfered and keep using its original npm module
name and repository. If a new module name needs to be created, it should preferably be
`@eslint-community/<the-old-name>`.

Automatic releases of the modules should be set up by the Core Team using the organization
secret in the GitHub organization.

Auxiliary projects can can be nominated to become a primary project by its Collaborators,
by opening a private team discussion [on GitHub](https://github.com/eslint-community/collaborators/discussions).

If a primary project is no longer widely depended upon, or have technical reasons to no
longer stay a primary project, the Core Team can decide to convert it into an auxiliary
project in discussion with its Collaborators.

## Project nominations

Projects that are widely depended upon within the ESLint ecosystem may be nominated to
become ESLint-Community projects by anyone by opening a public issue [on GitHub](https://github.com/eslint-community/governance).
The project should fulfill a few criterias:

The project should:

* Preferably be: An ESLint plugin or formatter
* Maybe be: A dependency used by an ESLint-Community project or the main ESLint repo
* Not be: Primarily an ESLint config

The project should also:

* be widely depended upon throughout the community (eg. 3M downloads/week or similar)
* have an OSI-approved license (preferably same as ESLint itself: MIT)
* have proposed Collaborators or have possibility to be deemed a Primary project
  by the Core Team

If project currently has an active maintainer it should be transfered and then:

* the current maintainer should be willing to transfer the project to ESLint-Community

If it's an abandoned project that needs to be forked:

* It shouldn't have received an update in a substantial amount of time (eg. last 6 months)
  or it should present a major obstacle to the adoption of eg. a new major version of ESLint
* A clear notice about the nomination should have been made to the project and its
  maintainer at least 30 days before it can be accepted

Projects should typically start out with a status of "auxiliary".

## Collaborator nominations

Individuals making significant and valuable contributions to a project may be
a candidate to join the ESLint-Community organization and that team.

An existing Collaborator needs to open a private team discussion [on GitHub](https://github.com/eslint-community/collaborators/discussions) and
list the candidates they want to sponsor with a link to the user's contributions. For
example:

* Activities in the ESLint-Community organization
  `[USERNAME](https://github.com/search?q=author:USERNAME+org:eslint-community)`

Otherwise, a Contributor may self-apply if they believe they meet the above
criteria by reaching out to a Core Team member privately with the links to their
valuable contributions. That Lead Maintainer will then open a private team discussion on
GitHub regarding that and reply back when a decision has been made.

The consensus to grant a new candidate Collaborator status is reached when:

- at least two of the Core Team members approve
- at least half of the current collaborators in that team approve, rounded up
  (and not counting Core Team members)

## Core Team nominations

A Team Member may be promoted to the Core Team only through nomination by a
Core Team member and with agreement from the rest of Core Team as well as the
ESLint TSC.

The ESLint TSC can appoint and revoke Core Team members at their own discretion.

## Consensus seeking process

The ESLint Community follows a Lazy [Consensus Seeking]() decision-making model,
inspired by the [ASF]().

_Lazy_ means that silence is consent if an appropriate amount of time has passed
(most of the time: at least a week) since the suggestion was made and no objections
has been raised.

This only holds true if all relevant parties has been notified of the suggestion
and given the opportunity to take part. Eg. extra care needs to be taken during
holiday and vacation times.

Decision makers should strive to give active consent and not actively wait out
silent consent.

### Votes

In case of a Collaborator objection to a specific change, the Core Team can
vote to override the objection if consensus can not be reached.

For all votes, a simple majority of all Core Team members for, or against, the
issue wins. A Core Team member may choose to participate in any vote through
abstention.

The ESLint TSC can decide to override / veto any decision / objection made by
Collaborators or Core Team. The ESLint Project decides how to arrive at
such decisions.

[Consensus Seeking]:
    https://en.wikipedia.org/wiki/Consensus-seeking_decision-making
[ASF]:
    https://community.apache.org/committers/decisionMaking.html
