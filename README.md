# eslint-plugin-firecloud

A proxy module to rules in [`eslint-config-firecloud`](https://github.com/rokmoln/eslint-config-firecloud).

This is a peer dependency of [`eslint-config-firecloud`](https://github.com/rokmoln/eslint-config-firecloud) that
points back to `eslint-config-firecloud/rules` module for a list of rules to be exported by this plugin.


## Why?

[ESLint](https://eslint.org/) is not very flexible about your own custom rules and the only working way to share
them across several repos is to create an `eslint-plugin-your-team-name` and put all the rules there.
Since, we already had our shared `eslint-config-firecloud`, we wanted to have our rules lying beside configs,
so both rules and configs for them can be changed in the same place. So this module acts as a sole proxy.


## License

[UNLICENSE](UNLICENSE)
