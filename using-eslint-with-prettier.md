| | [`prettier-eslint`](https://github.com/prettier/prettier-eslint) | [`eslint-plugin-prettier`](https://github.com/prettier/eslint-plugin-prettier) | [`eslint-config-prettier`](https://github.com/prettier/eslint-config-prettier) |
|--|:--:|:--:|:--:|
| What it is | A JavaScript module exporting a single function. | An ESLint plugin. | An ESLint configuration. |
| What it does | Runs the code (string) through `prettier` then `eslint --fix`. The output is also a string. | Plugins usually contain implementations for additional rules that ESLint will check for. This plugin uses Prettier under the hood and will raise ESLint errors when your code differs from Prettier's expected output. | This config turns off formatting-related rules that might conflict with Prettier, allowing you to use Prettier with other ESLint configs like [`eslint-config-airbnb`](https://www.npmjs.com/package/eslint-config-airbnb). | 
| How to use it | Either calling the function in your code or via [`prettier-eslint-cli`](https://github.com/prettier/prettier-eslint-cli) if you prefer the command line. | Add it to your `.eslintrc`. | Add it to your `.eslintrc`. |
| Is the final output Prettier compliant? | Depends on your ESLint config | Yes | Yes |
| Do you need to run `prettier` command separately? | No | No | Yes |
| Do you need to use anything else? | No | You may want to turn off conflicting rules using `eslint-config-prettier`. | No |
