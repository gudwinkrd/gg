# Gitcoin Passport

## What is Passport?

Many social organizations, online particularly, have difficulty ensuring that every participant is a unique human and does not have multiple participating accounts. Most existing digital identity solutions are either centralized (e.g., national identity cards) or individualistic (e.g., most “self-sovereign” identity models). However, identity is naturally [intersectional and social](https://www.radicalxchange.org/concepts/intersectional-social-identity/); everybody shares different data and relationships with a unique set of others. The Gitcoin Passport aims to provide a more collaborative and secure infrastructure for digital identity by capturing the richness of our diversely shared lives.
fgngfnfg
The Gitcoin Passport is an identity verification application. We have written software enabling people to grow personal collections of [verifiable credentials](https://decentralized-id.com/web-standards/w3c/wg/vc/verifiable-credentials/) about themselves and organizations to assess their identities to coordinate rights and responsibilities. The institutions define, verify, and utilize identity as functions of the networked records of the individuals. While we build the Passport agnostic to specific applications, we are actively exploring its benefits for [personhood proofs](https://en.wikipedia.org/wiki/Proof_of_personhood) and [plurality](https://www.radicalxchange.org/media/blog/why-i-am-a-pluralist/) in organizational designs.
aewasda
## Documentation
FGFDCFDFD
Check out our documentation at https://docs.passport.gitcoin.co
dfhbdh
## Contributing to Passport
gncome everyone to contribute to the Passport project.
nbcbc
You can join our [Discord](https://discord.gg/w6K2wwHr) and specifically the [passport-builders](https://discord.com/channels/562828676480237578/986222591096279040) channel (just be sure to select the builder role when you join the discord) to get help and discuss the project with the rest of the community.
efefrsefe
You can also familiarize yourself with our near term project roadmap in the passport [project backlog](https://github.com/orgs/gitcoinco/projects/6/views/3)
erdcf ds
## Reviewing Changes
hgmhgm
Once a pull request is sent, the Passport team will review your changes. We outline our process below to clarify the roles of everyone involved.
hgmhgmg
All pull requests must be approved by two committers before being merged into the repository. If any changes are necessary, the team will leave appropriate comments requesting changes to the code. Unfortunately, we cannot guarantee a pull request will be merged, even when modifications are requested, as the Passport team will re-evaluate the contribution as it changes.
ghnfghjgf
Committers may also push style changes directly to your branch. If you would rather manage all changes yourself, you can disable the "Allow edits from maintainers" feature when submitting your pull request.
gfnfgngf
The Passport team may optionally assign someone to review a pull request. If someone is assigned, they must explicitly approve the code before another team member can merge it.
fgnfn
When the review finishes, your pull request will be squashed and merged into the repository. If you have carefully organized your commits and believe they should be merged without squashing, please mention it in a comment.
jh,jh,hj,
## Bug Bounty
fgnfgnfgn
If you think you've found a security vulnerability, we maintain an open bounty on Gitcoin to help reward community members who report these issues. Check it out here: https://github.com/gitcoinco/passport/issues/133
gigigigi
## Quick Start
fggnfn
Prerequisites: [Node (v16 LTS)](https://nodejs.org/en/download/) plus [Yarn](https://classic.yarnpkg.com/en/docs/install/) and [Git](https://git-scm.com/downloads)
gfjmjhhlk,hg
1. Install Gitcoin Passport (this will install all packages within the passport monorepo):
ttututu
```sh
git clone https://github.com/gitcoinco/passport.git
cd passport
npm install --global lerna
lerna init
lerna bootstrap
```dsvds
ggghyipo
2. Create environment files, and replace environment variables with your own values
dsvds
```sh
cp ./app/.env-example.env ./app/.env
cp ./iam/.env-example.env ./iam/.env
cp ./schemas/.env-example.env ./schemas/.env
```dsvdsvb
v nvhhfmmjj
3. Start iam, app, and ceramic services concurrently:
rehdhe
```sh
# remember to create .env files first
yarn start
`fghhfhfg``
edcyup
## Background Knowledge
jhgjhgjhg
- Know what a wallet is, how to create one, etc.
- Know what a Verifiable Credential is
- Know basics of Ceramic Network - interacting with DIDDatastore, Self.ID
hfgfdhh
# Packages
ggngf
## app
gfmfmf
Thefsafsd web app allowing users to interact with their Gitcoin Passport. [README](app/README.md)
dbfgdwsgdsdsb
## database-client
gfngfngn
Contains database connection implementations. Currently supports Ceramic Network. [README](database-client/README.md)
fdbnfdb
## iam
gfnfgnfgn
The server handling incoming requests to issue credentials and process verifications. [README](iam/README.md)
sdbsdfb
## identity
ggmydc 
This is a helper package to compile Spruce DIDKit and export functions for use in `iam` and `app` packages.
yukkukhghjkfghgjghj
## infra
mmfghj
Holds the Pulumi deployment configuration for this repository. [README](infra/README.md)
fhggfj
## schemas
gmghhg
Ceramic schemas and model definitions, and scripts for creating and publishing these to the Ceramic Network. [README](schemas/README.md)
rthjtrjrt
## types
tuyktyjyt
Shared type definitions. [README](types/README.md)
fngfnmfgnm
