##Instructions to setup a Hyperledger Indy Node

Clone repo and setup the Indy Pool

1. `git clone git@github.com:hyperledger/indy-sdk.git`
2. `docker build -f ci/indy-pool.dockerfile -t indy_pool .`
3. `docker run -itd -p 9701-9708:9701-9708 indy_pool`
4. `docker run -it indy_pool /bin/bash`

Login to Indy Pool container go to Indy Console

5. `docker run -it indy_pool /bin/bash`
6. `indy@15102e588e89:/$ indy`

You should end up in a console below
```
Indy-CLI (c) 2017 Evernym, Inc.
Type 'help' for more information.
Running Indy 1.6.576

indy>
```
