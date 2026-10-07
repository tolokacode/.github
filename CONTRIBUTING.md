# Contributing

Thanks for helping! Every contribution counts: a bug report, an idea, a typo fix or code.

## Questions and ideas

Open an issue and pick a template. Security problems are different: please report them
privately, see [SECURITY.md](SECURITY.md).

## How to contribute

1. **Open an issue first.** Describe what you want to change and why. This way we agree on
   the solution before you spend time on code.
2. **Fork and branch.** Fork the repository and name your branch after the issue, for example `12-fix-refund`.
3. **Open a pull request.** Fill in the template: the issue number, what you changed, **why**,
   and how you tested it.
4. **Review.** A maintainer looks at your code. If it's fine, it gets merged into `main`.
   If not, you'll get comments and can push fixes to the same branch.

## Code

- Keep it simple. No clever tricks or extra layers.
- Only add comments where the reason isn't obvious from the code.
- Test your change. Each repository's README explains how.

## Commits

Start the first line with the issue number and keep it short. Add details below an empty line if needed:

```
#12 Fix refund for partial amount

Refund used the full order total instead of the entered amount.
```

## Sign your commits (DCO)

Every commit needs a `Signed-off-by` line. It says you wrote the code and have the right to
share it under the project's license ([Developer Certificate of Origin](https://developercertificate.org/)).
The name and email must match the commit author.

Git adds it for you with `-s`:

```bash
git commit -s -m "#12 Fix refund for partial amount"
```

Forgot? If you haven't pushed yet, run `git commit --amend -s --no-edit`.
If you already pushed several commits, run `git rebase --signoff main` and then `git push --force-with-lease`.

## Releases

`main` always works. We tag versions with [Semantic Versioning](https://semver.org/):
`0.1.0`, then `0.1.1` for a fix, `0.2.0` for a new feature.

## License

By contributing, you agree that your work is shared under the license of that repository:
[EUPL-1.2](https://interoperable-europe.ec.europa.eu/collection/eupl/eupl-text-eupl-12) for plugins and apps, [MIT](https://opensource.org/license/mit) for libraries.
Each repository has its license in the `LICENSE` file.
