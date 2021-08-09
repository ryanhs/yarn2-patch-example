> this is yarn 2

## Yarn Patch learn, example: superagent

1. `yarn patch superagent`
1. into file: (see main file in package.json)
    ```
    // test
    request.patchedAt = '2021-08-09';
    ```

1. patch commit, example
    `yarn patch-commit /tmp/xfs-59ea403b > patches/superagent.patch`

1. change package.json
    ```
    "superagent": "patch:superagent@6.1.0#patches/superagent.patch"
    ```

1. `yarn` again

1. see again, `yarn node ./index.js`



#### yarn 2 gitignore

[https://yarnpkg.com/getting-started/qa#which-files-should-be-gitignored]()

```

```


#### refs for yarn 1

- [https://callstack.com/blog/say-goodbye-to-old-fashioned-forks-thanks-to-the-patch-package/]()
- [https://www.ryanelainska.com/how-to-patch-an-npm-package-with-yarn-patch]()
