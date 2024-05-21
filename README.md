---
title: About billing for GitHub Actions
intro: 'If you want to use {{ site.data.variables.product.prodname_actions }} beyond the storage or minutes included in your account, you will be billed for additional usage.'
product: '{{ site.data.reusables.gated-features.actions }}'
versions:
  free-pro-team: '*'
---

### About billing for {{ site.data.variables.product.prodname_actions }}

{{ site.data.reusables.github-actions.actions-billing }} {{ site.data.reusables.github-actions.actions-spending-limit }}

Minutes reset every month, while storage usage does not.

|Product | Storage | Minutes (per month)|
|------- | ------- | ---------|
| {{ site.data.variables.product.prodname_free_user }} | 500 MB | 2,000 |
| {{ site.data.variables.product.prodname_pro }} | 1 GB | 3,000 |
| {{ site.data.variables.product.prodname_free_team }} for organizations | 500 MB | 2,000 |
| {{ site.data.variables.product.prodname_team }} | 2 GB | 3,000 |
| {{ site.data.variables.product.prodname_ghe_cloud }} | 50 GB | 50,000 |

Jobs that run on Windows and macOS runners that {{ site.data.variables.product.prodname_dotcom }} hosts consume minutes at 2 and 10 times the rate that jobs on Linux runners consume. For example, using 1,000 Windows minutes would consume 2,000 of the minutes included in your account. Using 1,000 macOS minutes, would consume 10,000 minutes included in your account.

| Operating system | Minute multiplier |
|------- | ---------|
| Linux | 1 |
| macOS| 10 |
| Windows | 2 |

The storage used by a repository is the total storage used by {{ site.data.variables.product.prodname_actions }} artifacts and {{ site.data.variables.product.prodname_registry }}. Your storage cost is the total usage for all repositories owned by your account. For more information about pricing for  {{ site.data.variables.product.prodname_registry }}, see "[About billing for {{ site.data.variables.product.prodname_registry }}](/github/setting-up-and-managing-billing-and-payments-on-github/about-billing-for-github-packages)."

 If your account's usage surpasses these limits and you have set a spending limit above $0, you will pay $0.25 USD per GB of storage per month and per-minute usage depending on the operating system used by the {{ site.data.variables.product.prodname_dotcom }}-hosted runner. {{ site.data.variables.product.prodname_dotcom }} rounds the minutes each job uses up to the nearest minute.

{% note %}

**Note:** Minute multipliers do not apply to the per-minute rates shown below.

{% endnote %}

| Operating system | Per-minute rate |
|------- | ---------|
| Linux | $0.008 |
| macOS | $0.08 |
| Windows | $0.016 |

The number of jobs you can run concurrently across all repositories in your user or organization account depends on your GitHub plan. For more information, see "[Usage limits and billing](/actions/reference/usage-limits-billing-and-administration)" for {{ site.data.variables.product.prodname_dotcom }}-hosted runners and "[About self-hosted runners](/actions/hosting-your-own-runners/about-self-hosted-runners/#usage-limits)" for self-hosted runner usage limits.

### Calculating minute and storage spending

At the end of the month, {{ site.data.variables.product.prodname_dotcom }} calculates the cost of minutes and storage used over the amount included in your account. For example, if your organization uses {{ site.data.variables.product.prodname_team }} and allows unlimited spending, using 15,000 minutes could have a total storage and minute overage cost of $56, depending on the operating systems used to run jobs.

- 5,000 (3,000 Linux and 2,000 Windows) minutes = $56 ($24 + $32).
  - 3,000 Linux minutes at $0.008 per = $24.
  - 2,000 Windows minutes at $0.016 per minute = $32.

At the end of the month, {{ site.data.variables.product.prodname_dotcom }} rounds your data transfer to the nearest GB.

{{ site.data.variables.product.prodname_dotcom }} calculates your storage usage for each month based on hourly usage during that month. For example, if you use 3 GB of storage for 10 days of March and 12 GB for 21 days of March, your storage usage would be:

- 3 GB x 10 days x (24 hours per day) = 720 GB-Hours
- 12 GB x 21 days x (24 hours per day) = 6,048 GB-Hours
- 720 GB-Hours + 6,048 GB-Hours = 6,768 GB-Hours
- 6,768 GB-Hours / (744 hours per month) = 9.0967 GB-Months

At the end of the month, {{ site.data.variables.product.prodname_dotcom }} rounds your storage to the nearest MB. Therefore, your storage usage for March would be 9.097 GB.

Your {{ site.data.variables.product.prodname_actions }} usage shares your account's existing billing date, payment method, and receipt. {{ site.data.reusables.dotcom_billing.view-all-subscriptions }}

### About spending limits

By default, your account will have a spending limit of $0 for {{ site.data.variables.product.prodname_actions }} usage. To enable using minutes and storage for private repositories beyond the amounts included with your account, you can increase the spending limit or allow unlimited spending. For more information, see "[Managing your spending limit for {{ site.data.variables.product.prodname_actions }}](/github/setting-up-and-managing-billing-and-payments-on-github/managing-your-spending-limit-for-github-actions)."

{{ site.data.reusables.github-actions.spending-limit-enterprise-account }}

{{ site.data.reusables.dotcom_billing.actions-packages-unpaid-account }}# GitHub Docs <!-- omit in toc -->
[![Build GitHub Docs On Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new/?repo=github)

This repository contains the documentation website code and Markdown source files for [docs.github.com](https://docs.github.com).

GitHub's Docs team works on pre-production content in a private repo that regularly syncs with this public repo.

Use the table of contents icon <img alt="Table of contents icon" src="./contributing/images/table-of-contents.png" width="25" height="25" /> on the top right corner of this document to navigate to a specific section quickly.

## Contributing

We accept different types of contributions, including some that don't require you to write a single line of code. For detailed instructions on how to get started with our project, see "[About contributing to GitHub Docs](https://docs.github.com/en/contributing/collaborating-on-github-docs/about-contributing-to-github-docs)."

### Ways to contribute

On the GitHub Docs site, you can contribute by clicking the **Make a contribution** button at the bottom of the page to open a pull request for quick fixes like typos, updates, or link fixes.

You can also contribute by creating a local environment or opening a Codespace. For more information, see "[Setting up your environment to work on GitHub Docs](https://docs.github.com/en/contributing/setting-up-your-environment-to-work-on-github-docs)."

<img alt="Contribution call-to-action" src="./contributing/images/contribution_cta.png" width="400">

For more complex contributions, please open an issue using the most appropriate [issue template](https://github.com/github/docs/issues/new/choose) to describe the changes you'd like to see.

If you're looking for a way to contribute, you can scan through our [help wanted board](https://github.com/github/docs/issues?q=is%3Aopen+is%3Aissue+label%3A%22help+wanted%22) to find open issues already approved for work.

### And that's it!

If you're having trouble with your GitHub account, contact [Support](https://support.github.com).

That's how you can easily become a member of the GitHub Docs community. :sparkles:

## READMEs

In addition to the README you're reading right now, this repo includes other READMEs that describe the purpose of each subdirectory in more detail:

- [content/README.md](content/README.md)
- [content/graphql/README.md](content/graphql/README.md)
- [content/rest/README.md](content/rest/README.md)
- [contributing/README.md](contributing/README.md)
- [data/README.md](data/README.md)
- [data/reusables/README.md](data/reusables/README.md)
- [data/variables/README.md](data/variables/README.md)
- [src/README.md](src/README.md)

## License

The GitHub product documentation in the assets, content, and data folders are licensed under a [CC-BY license](LICENSE).

All other code in this repository is licensed under the [MIT license](LICENSE-CODE).

When using the GitHub logos, be sure to follow the [GitHub logo guidelines](https://github.com/logos).

## Thanks :purple_heart:

Thanks for all your contributions and efforts towards improving the GitHub documentation. We thank you for being part of our :sparkles: community :sparkles:!
