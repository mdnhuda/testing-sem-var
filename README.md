# build the custom plugin in ~/Projects/other/test-semantic-release/commit-analyzer-lister
$ yarn pack

# (once) export necessary tokens as ENV variable
 export GITHUB_TOKEN=....

# install the local plugin 
 $ npm install ../commit-analyzer-lister/sem-var-commit-analyzer-lister-...tar.gz

# add the local plugin in the .releaserc file
    "plugins": [
        ...
        "sem-var-commit-analyzer-lister"
    ],

# execute `semantic-release`
 $ npx semantic-release

-- just a comment