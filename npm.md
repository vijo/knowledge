# [](#npm)npm

## [](#passing-args-into-npm-run-scripts)passing args into npm run-scripts

If you've got a package.json like:

    ...
    "scripts": {
      "lint": "eslint src"
    }
    ...

and you want to run `eslint` with a different formatter, use the `--` separator followed by the args you want to run `eslint` with:

    npm run lint -- --format unix
