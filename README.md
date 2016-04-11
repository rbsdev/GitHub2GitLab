# GitHub2GitLab

Bash script to push tags and commits from all branches from GitHub to GitLab.

## Usage

Pass a list of repositories names to get started:

```bash
./migrate < repositories
```

For each repository, `migrate` will:

1. Clone
2. Fetch
3. Checkout every branch
4. Add a `gitlab` remote
5. Push everything to `gitlab`

Later, you might want to update the GitLab repository, for that just run:

```bash
./update < repositories
```

For each repository, `update` will:

1. Fetch and pull from `github`
2. Push everything to `gitlab`
