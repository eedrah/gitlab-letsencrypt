# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [3.0.0] - 2018-01-14

### Added
- Certificates are now automatically configured on a GitLab Page by using GitLab's API.
Full automation is now possible!
- Support for arbitrary GitLab instances, not just https://gitlab.com.

### Changed
- To prevent accidental rate-limiting, staging certificates are obtained by default. Use `--production` to obtain real certificates.
- `--repository` now accepts a full repository URL instead of a repository identifier.
- Commits made from `gitlab-le` now have their author set to "gitlab-le".
- Minimum required Node version is now 8.x.