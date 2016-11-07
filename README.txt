workflow to encrypt git repo contents

before anything, set password in .gitencrypt/* and cp -r .gitencrypt ~

before commiting, cp .gitattributes <repo> && cat config >> <repo>/.git/config

after cloning, cp .gitattributes <repo> && cd <repo> && git reset --hard HEAD

see https://github.com/aj-michael/gitencrypt/tree/encrypted for an example

credits to https://gist.github.com/shadowhand/873637
