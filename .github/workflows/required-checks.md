# Required Pull Request Checks & Troubleshooting

OpenSearch uses a variety of automated checks to ensure code quality, compatibility, and documentation standards. Some of these checks are displayed "below the fold" on the PR page or as comments, making them easy to overlook. This guide consolidates all required checks and provides links to documentation and troubleshooting steps.

---

## Required Checks Before Merge

| Check Name                | Description                                               | Troubleshooting / Docs                                  |
|---------------------------|-----------------------------------------------------------|---------------------------------------------------------|
| **Gradle Assemble**       | Builds the project on all supported platforms and JDKs.   | [Build Troubleshooting](../../CONTRIBUTING.md#build)       |
| **Gradle Precommit**      | Runs code style, static analysis, and basic tests.        | [Precommit Guide](../../CONTRIBUTING.md#precommit)         |
| **Changelog Verifier**    | Ensures changelog is updated unless skipped.              | [Changelog Guide](../../CONTRIBUTING.md#changelog)         |
| **Benchmark PR**          | Runs performance benchmarks on request.                   | [Benchmarks](../PERFORMANCE_BENCHMARKS.md)              |
| **Detect Breaking Change**| Checks for Java API compatibility breaks.                 | [API Compatibility](../../CONTRIBUTING.md#api)             |
| **Wrapper Validation**    | Validates Gradle wrapper integrity.                       | [Gradle Wrapper](https://docs.gradle.org/current/userguide/gradle_wrapper.html) |
| **Backport**              | Automates backporting merged PRs to other branches.       | [Backporting](../../CONTRIBUTING.md#backport)              |
| **Dependabot PR Actions** | Ensures dependency updates are properly handled.          | [Dependabot](https://docs.github.com/en/code-security/supply-chain-security/keeping-your-dependencies-updated-automatically/about-dependabot-version-updates) |
| **Link Checker**          | Checks for broken links in documentation.                 | [Link Checker](https://github.com/lycheeverse/lychee)   |
| **Stalled PRs**           | Labels PRs with no activity for 30 days as stalled.       | [Stalled PRs](../../CONTRIBUTING.md#stalled)               |

---

## What to Do If a Check Fails

1. **Expand the failed check** in the PR checks section to view logs and error messages.
2. **Consult the documentation** linked above for common issues and solutions.
3. **Ask for help** by commenting on the PR or reaching out in the community channels.

---

## Additional Resources

- [OpenSearch Contributing Guide](../CONTRIBUTING.md)
- [Performance Benchmarks](../PERFORMANCE_BENCHMARKS.md)
- [OpenSearch Documentation](https://opensearch.org/docs/latest/)

---

*Maintainers: Please keep this document up to date as workflows change.*