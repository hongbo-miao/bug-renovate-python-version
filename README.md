# bug-renovate-python-version

## Introduction

### Observed behavior

`.python-version` is used by [Pyenv](https://github.com/pyenv/pyenv).

Renovate opened pull request with title "chore(deps): update python docker tag to v3.11.1".

### Expected behavior

Renovate should either

- open pull request with correct title
- or ignore updating this file (?) as this file [most time needs to be git ignored](https://stackoverflow.com/questions/54315206/should-we-gitignore-the-python-version-file)

## Ticket

Opened the ticket at https://github.com/renovatebot/renovate/issues/19470

## Renovate Log

<details>
  <summary>Click to expand</summary>

  ```shell
DEBUG: No dangling containers to remove
INFO: Repository started
{
  "renovateVersion": "34.62.1"
}
DEBUG: Using localDir: /mnt/renovate/gh/Hongbo-Miao/bug-renovate-python-version
DEBUG: PackageFiles.clear() - Package files deleted
DEBUG: initRepo("Hongbo-Miao/bug-renovate-python-version")
DEBUG: Using queue: host=api.github.com, concurrency=10
DEBUG: Hongbo-Miao/bug-renovate-python-version default branch = main
DEBUG: Using app token for git init
DEBUG: RepoCacheBase.load() - expecting data of type 'string' received 'object' instead - skipping
DEBUG: Resetting npmrc
DEBUG: checkOnboarding()
DEBUG: isOnboarded()
DEBUG: findFile(renovate.json)
DEBUG: Initializing git repository into /mnt/renovate/gh/Hongbo-Miao/bug-renovate-python-version
DEBUG: Performing blobless clone
DEBUG: git clone completed
{
  "durationMs": 981
}
DEBUG: latest repository commit
{
  "latestCommit": {
    "hash": "22206412ee0bd3b0b08d8769057fb88de273b484",
    "date": "2022-12-18T17:10:26-08:00",
    "message": "feat: init",
    "refs": "HEAD -> main, origin/main, origin/HEAD",
    "body": "",
    "author_name": "Hongbo Miao",
    "author_email": "Hongbo.Miao@outlook.com"
  }
}
DEBUG: findFile(renovate.json5)
DEBUG: Config file exists, fileName: renovate.json5
DEBUG: Retrieving issueList
DEBUG: Retrieved 0 issues
DEBUG: Repo is onboarded
DEBUG: Found renovate.json5 config file
DEBUG: Repository config
{
  "fileName": "renovate.json5",
  "config": {
    "extends": [
      "config:base"
    ]
  }
}
DEBUG: migrateAndValidate()
DEBUG: No config migration necessary
DEBUG: massaged config
{
  "config": {
    "extends": [
      "github>whitesource/merge-confidence:beta",
      "config:base"
    ]
  }
}
DEBUG: migrated config
{
  "config": {
    "extends": [
      "github>whitesource/merge-confidence:beta",
      "config:base"
    ]
  }
}
DEBUG: Setting hostRules from config
DEBUG: Found repo ignorePaths
{
  "ignorePaths": [
    "**/node_modules/**",
    "**/bower_components/**",
    "**/vendor/**",
    "**/examples/**",
    "**/__tests__/**",
    "**/test/**",
    "**/tests/**",
    "**/__fixtures__/**"
  ]
}
DEBUG: Using queue: host=api.github.com, concurrency=10
DEBUG: No vulnerability alerts found
DEBUG: No vulnerability alerts found
DEBUG: findIssue(Dependency Dashboard)
DEBUG: No baseBranches
DEBUG: extract()
DEBUG: Setting current branch to main
DEBUG: latest commit
{
  "branchName": "main",
  "latestCommitDate": "2022-12-18T17:10:26-08:00"
}
DEBUG: Using file match: (^|/)tasks/[^/]+\.ya?ml$ for manager ansible
DEBUG: Using file match: (^|/)requirements\.ya?ml$ for manager ansible-galaxy
DEBUG: Using file match: (^|/)galaxy\.ya?ml$ for manager ansible-galaxy
DEBUG: Using file match: (^|/)\.tool-versions$ for manager asdf
DEBUG: Using file match: azure.*pipelines?.*\.ya?ml$ for manager azure-pipelines
DEBUG: Using file match: (^|/)batect(-bundle)?\.yml$ for manager batect
DEBUG: Using file match: (^|/)batect$ for manager batect-wrapper
DEBUG: Using file match: (^|/)WORKSPACE(|\.bazel)$ for manager bazel
DEBUG: Using file match: \.bzl$ for manager bazel
DEBUG: Using file match: (^|\/)\.bazelversion$ for manager bazelisk
DEBUG: Using file match: (^|/)\.?bitbucket-pipelines\.ya?ml$ for manager bitbucket-pipelines
DEBUG: Using file match: buildkite\.ya?ml for manager buildkite
DEBUG: Using file match: \.buildkite/.+\.ya?ml$ for manager buildkite
DEBUG: Using file match: (^|/)Gemfile$ for manager bundler
DEBUG: Using file match: \.cake$ for manager cake
DEBUG: Using file match: (^|/)Cargo\.toml$ for manager cargo
DEBUG: Using file match: (^|/)\.circleci/config\.yml$ for manager circleci
DEBUG: Using file match: (^|/)cloudbuild\.ya?ml for manager cloudbuild
DEBUG: Using file match: (^|/)Podfile$ for manager cocoapods
DEBUG: Using file match: (^|/)([\w-]*)composer\.json$ for manager composer
DEBUG: Using file match: (^|/)conanfile\.(txt|py)$ for manager conan
DEBUG: Using file match: (^|/)(?:deps|bb)\.edn$ for manager deps-edn
DEBUG: Using file match: (^|/)(?:docker-)?compose[^/]*\.ya?ml$ for manager docker-compose
DEBUG: Using file match: (^|/|\.)Dockerfile$ for manager dockerfile
DEBUG: Using file match: (^|/)Dockerfile[^/]*$ for manager dockerfile
DEBUG: Using file match: (^|/)\.drone\.yml$ for manager droneci
DEBUG: Using file match: (^|/)fleet\.ya?ml for manager fleet
DEBUG: Using file match: (^|\/)flux-system\/(?:.+\/)?gotk-components\.yaml$ for manager flux
DEBUG: Using file match: (^|\/)\.fvm\/fvm_config\.json$ for manager fvm
DEBUG: Using file match: (^|/)\.gitmodules$ for manager git-submodules
DEBUG: Using file match: ^(workflow-templates|\.github\/workflows)\/[^/]+\.ya?ml$ for manager github-actions
DEBUG: Using file match: (^|\/)action\.ya?ml$ for manager github-actions
DEBUG: Using file match: \.gitlab-ci\.yml$ for manager gitlabci
DEBUG: Using file match: \.gitlab-ci\.yml$ for manager gitlabci-include
DEBUG: Using file match: (^|/)go\.mod$ for manager gomod
DEBUG: Using file match: \.gradle(\.kts)?$ for manager gradle
DEBUG: Using file match: (^|\/)gradle\.properties$ for manager gradle
DEBUG: Using file match: (^|\/)gradle\/.+\.toml$ for manager gradle
DEBUG: Using file match: \.versions\.toml$ for manager gradle
DEBUG: Using file match: (^|\/)versions.props$ for manager gradle
DEBUG: Using file match: (^|\/)versions.lock$ for manager gradle
DEBUG: Using file match: (^|/)gradle/wrapper/gradle-wrapper\.properties$ for manager gradle-wrapper
DEBUG: Using file match: (^|/)requirements\.yaml$ for manager helm-requirements
DEBUG: Using file match: (^|/)values\.yaml$ for manager helm-values
DEBUG: Using file match: (^|/)helmfile\.yaml$ for manager helmfile
DEBUG: Using file match: (^|/)Chart\.yaml$ for manager helmv3
DEBUG: Using file match: (^|/)bin/hermit$ for manager hermit
DEBUG: Using file match: ^Formula/[^/]+[.]rb$ for manager homebrew
DEBUG: Using file match: \.html?$ for manager html
DEBUG: Using file match: (^|/)plugins\.(txt|ya?ml)$ for manager jenkins
DEBUG: Using file match: (^|/)jsonnetfile\.json$ for manager jsonnet-bundler
DEBUG: Using file match: ^.+\.main\.kts$ for manager kotlin-script
DEBUG: Using file match: (^|/)kustomization\.ya?ml$ for manager kustomize
DEBUG: Using file match: (^|/)project\.clj$ for manager leiningen
DEBUG: Using file match: (^|/|\.)pom\.xml$ for manager maven
DEBUG: Using file match: ^(((\.mvn)|(\.m2))/)?settings\.xml$ for manager maven
DEBUG: Using file match: (^|/)package\.js$ for manager meteor
DEBUG: Using file match: (^|\/)Mintfile$ for manager mint
DEBUG: Using file match: (^|/)mix\.exs$ for manager mix
DEBUG: Using file match: (^|\/)flake\.nix$ for manager nix
DEBUG: Using file match: (^|/)\.node-version$ for manager nodenv
DEBUG: Using file match: (^|/)package\.json$ for manager npm
DEBUG: Using file match: \.(?:cs|fs|vb)proj$ for manager nuget
DEBUG: Using file match: \.(?:props|targets)$ for manager nuget
DEBUG: Using file match: (^|\/)dotnet-tools\.json$ for manager nuget
DEBUG: Using file match: (^|\/)global\.json$ for manager nuget
DEBUG: Using file match: (^|/)\.nvmrc$ for manager nvm
DEBUG: Using file match: (^|/)([\w-]*)requirements\.(txt|pip)$ for manager pip_requirements
DEBUG: Using file match: (^|/)setup\.py$ for manager pip_setup
DEBUG: Using file match: (^|/)Pipfile$ for manager pipenv
DEBUG: Using file match: (^|/)pyproject\.toml$ for manager poetry
DEBUG: Using file match: (^|/)\.pre-commit-config\.yaml$ for manager pre-commit
DEBUG: Using file match: (^|/)pubspec\.ya?ml$ for manager pub
DEBUG: Using file match: (^|\/)Puppetfile$ for manager puppet
DEBUG: Using file match: (^|/)\.python-version$ for manager pyenv
DEBUG: Using file match: (^|/)\.ruby-version$ for manager ruby-version
DEBUG: Using file match: \.sbt$ for manager sbt
DEBUG: Using file match: project/[^/]*.scala$ for manager sbt
DEBUG: Using file match: (^|/)setup\.cfg$ for manager setup-cfg
DEBUG: Using file match: (^|/)Package\.swift for manager swift
DEBUG: Using file match: \.tf$ for manager terraform
DEBUG: Using file match: (^|/)\.terraform-version$ for manager terraform-version
DEBUG: Using file match: (^|/)terragrunt\.hcl$ for manager terragrunt
DEBUG: Using file match: (^|/)\.terragrunt-version$ for manager terragrunt-version
DEBUG: Using file match: \.tflint\.hcl$ for manager tflint-plugin
DEBUG: Using file match: ^\.travis\.yml$ for manager travis
DEBUG: Using file match: (^|/)\.vela\.ya?ml$ for manager velaci
DEBUG: Using file match: (^|\/)\.woodpecker[^/]*\.ya?ml$ for manager woodpecker
DEBUG: Matched 1 file(s) for manager pyenv: .python-version
DEBUG: Found pyenv package files
DEBUG: Found 1 package file(s)
INFO: Dependency extraction complete
{
  "baseBranch": "main",
  "stats": {
    "managers": {
      "pyenv": {
        "fileCount": 1,
        "depCount": 1
      }
    },
    "total": {
      "fileCount": 1,
      "depCount": 1
    }
  }
}
DEBUG: PackageFiles.add() - Package file saved for base branch
{
  "baseBranch": "main"
}
DEBUG: Package releases lookups complete
{
  "baseBranch": "main"
}
DEBUG: branchifyUpgrades
DEBUG: detectSemanticCommits()
DEBUG: getCommitMessages
DEBUG: semanticCommits: detected "angular"
DEBUG: semanticCommits: enabled
DEBUG: 1 flattened updates found: python
DEBUG: Returning 1 branch(es)
DEBUG: config.repoIsOnboarded=true
DEBUG: packageFiles with updates
{
  "baseBranch": "main",
  "config": {
    "pyenv": [
      {
        "packageFile": ".python-version",
        "deps": [
          {
            "depName": "python",
            "currentValue": "3.10.9",
            "datasource": "docker",
            "depIndex": 0,
            "updates": [
              {
                "bucket": "non-major",
                "newVersion": "3.11.1",
                "newValue": "3.11.1",
                "newMajor": 3,
                "newMinor": 11,
                "updateType": "minor",
                "branchName": "renovate/python-3.x"
              }
            ],
            "warnings": [],
            "versioning": "docker",
            "registryUrl": "https://index.docker.io",
            "currentVersion": "3.10.9",
            "isSingleVersion": true,
            "fixedVersion": "3.10.9"
          }
        ]
      }
    ]
  }
}
DEBUG: detectSemanticCommits()
DEBUG: semanticCommits: returning "enabled" from cache
DEBUG: processRepo()
DEBUG: Processing 1 branch: renovate/python-3.x
DEBUG: Calculating hourly PRs remaining
DEBUG: getPrList success
{
  "pullsTotal": 0,
  "requestsTotal": 1,
  "apiQuotaAffected": true
}
DEBUG: currentHourStart=2022-12-19T01:00:00.000+00:00
DEBUG: PR hourly limit remaining: 2
DEBUG: Calculating prConcurrentLimit (10)
DEBUG: getBranchPr(renovate/python-3.x)
DEBUG: findPr(renovate/python-3.x, undefined, open)
DEBUG: findPr(renovate/python-3.x, undefined, closed)
DEBUG: 0 PRs are currently open
DEBUG: PR concurrent limit remaining: 10
DEBUG: Calculated maximum PRs remaining this run: 2
DEBUG: PullRequests limit = 2
DEBUG: Calculating hourly PRs remaining
DEBUG: currentHourStart=2022-12-19T01:00:00.000+00:00
DEBUG: PR hourly limit remaining: 2
DEBUG: Calculating branchConcurrentLimit (10)
DEBUG: 0 already existing branches found:
DEBUG: Branch concurrent limit remaining: 10
DEBUG: Calculated maximum branches remaining this run: 2
DEBUG: Branches limit = 2
DEBUG: syncBranchState()(branch="renovate/python-3.x")
DEBUG: syncBranchState(): Branch cache not found, creating minimal branchState(branch="renovate/python-3.x")
DEBUG: getBranchPr(renovate/python-3.x)(branch="renovate/python-3.x")
DEBUG: findPr(renovate/python-3.x, undefined, open)(branch="renovate/python-3.x")
DEBUG: findPr(renovate/python-3.x, undefined, closed)(branch="renovate/python-3.x")
DEBUG: branchExists=false(branch="renovate/python-3.x")
DEBUG: dependencyDashboardCheck=undefined(branch="renovate/python-3.x")
DEBUG: recreateClosed is false(branch="renovate/python-3.x")
DEBUG: findPr(renovate/python-3.x, chore(deps): update python docker tag to v3.11.1, !open)(branch="renovate/python-3.x")
DEBUG: prAlreadyExisted=false(branch="renovate/python-3.x")
DEBUG: Checking schedule(at any time, null)(branch="renovate/python-3.x")
DEBUG: No schedule defined(branch="renovate/python-3.x")
DEBUG: Branch needs creating(branch="renovate/python-3.x")
DEBUG: Using reuseExistingBranch: false(branch="renovate/python-3.x")
DEBUG: Setting current branch to main(branch="renovate/python-3.x")
DEBUG: latest commit(branch="renovate/python-3.x")
{
  "branchName": "main",
  "latestCommitDate": "2022-12-18T17:10:26-08:00"
}
DEBUG: manager.getUpdatedPackageFiles() reuseExistingBranch=false(branch="renovate/python-3.x")
DEBUG: Starting search at index 0(packageFile=".python-version", branch="renovate/python-3.x")
{
  "depName": "python"
}
DEBUG: Found match at index 0(packageFile=".python-version", branch="renovate/python-3.x")
{
  "depName": "python"
}
DEBUG: Contents updated(packageFile=".python-version", branch="renovate/python-3.x")
{
  "depName": "python"
}
DEBUG: Updated 1 package files(branch="renovate/python-3.x")
DEBUG: No updated lock files in branch(branch="renovate/python-3.x")
DEBUG: 1 file(s) to commit(branch="renovate/python-3.x")
DEBUG: Preparing files for committing to branch renovate/python-3.x(branch="renovate/python-3.x")
DEBUG: Setting git author name: Renovate Bot(branch="renovate/python-3.x")
DEBUG: Setting git author email: bot@renovateapp.com(branch="renovate/python-3.x")
DEBUG: git commit(branch="renovate/python-3.x")
{
  "deletedFiles": [],
  "ignoredFiles": [],
  "result": {
    "author": null,
    "branch": "renovate/python-3.x",
    "commit": "e754d1b45265d78bf60334d94df3eefc60bf6b12",
    "root": false,
    "summary": {
      "changes": 1,
      "insertions": 1,
      "deletions": 1
    }
  }
}
DEBUG: resetToCommit(22206412ee0bd3b0b08d8769057fb88de273b484)(branch="renovate/python-3.x")
DEBUG: Fetching branch renovate/python-3.x(branch="renovate/python-3.x")
INFO: Branch created(branch="renovate/python-3.x")
{
  "commitSha": "ed82288aaebbe067d366d856c2ec611690e4a94f"
}
DEBUG: Ensuring PR(branch="renovate/python-3.x")
DEBUG: There are 0 errors and 0 warnings(branch="renovate/python-3.x")
DEBUG: getBranchPr(renovate/python-3.x)(branch="renovate/python-3.x")
DEBUG: findPr(renovate/python-3.x, undefined, open)(branch="renovate/python-3.x")
DEBUG: findPr(renovate/python-3.x, undefined, closed)(branch="renovate/python-3.x")
DEBUG: Creating PR(branch="renovate/python-3.x")
{
  "prTitle": "chore(deps): update python docker tag to v3.11.1"
}
DEBUG: Creating PR(branch="renovate/python-3.x")
{
  "title": "chore(deps): update python docker tag to v3.11.1",
  "head": "Hongbo-Miao:renovate/python-3.x",
  "base": "main",
  "draft": false
}
DEBUG: PR created(branch="renovate/python-3.x")
{
  "pr": 1,
  "draft": false
}
DEBUG: Adding labels '' to #1(branch="renovate/python-3.x")
INFO: PR created(branch="renovate/python-3.x")
{
  "pr": 1,
  "prTitle": "chore(deps): update python docker tag to v3.11.1"
}
DEBUG: addParticipants(pr=1)(branch="renovate/python-3.x")
DEBUG: Created Pull Request #1(branch="renovate/python-3.x")
DEBUG: PR is not configured for automerge(branch="renovate/python-3.x")
DEBUG: setBranchCommit()(branch="renovate/python-3.x")
DEBUG: getBranchPr(renovate/python-3.x)
DEBUG: findPr(renovate/python-3.x, undefined, open)
DEBUG: Found PR #1
DEBUG: branch.isBehindBase(): using cached result "false"
DEBUG: isBranchConflicted(main, renovate/python-3.x)
DEBUG: branch.isConflicted(): using cached result "false"
DEBUG: Ensuring Dependency Dashboard
DEBUG: ensureIssue(Dependency Dashboard)
INFO: Issue created
DEBUG: Removing any stale branches
DEBUG: config.repoIsOnboarded=true
DEBUG: Branch lists
{
  "branchList": [
    "renovate/python-3.x"
  ],
  "renovateBranches": [
    "renovate/python-3.x"
  ]
}
DEBUG: remainingBranches=
DEBUG: No branches to clean up
DEBUG: Retrieving issueList
DEBUG: Retrieved 1 issues
DEBUG: Cleaning up Renovate refs: refs/renovate/*
DEBUG: PackageFiles.clear() - Package files deleted
DEBUG: Branch summary
{
  "baseBranches": [
    {
      "branchName": "main",
      "sha": "22206412ee0bd3b0b08d8769057fb88de273b484"
    }
  ],
  "branches": [
    {
      "automerge": false,
      "baseBranch": "main",
      "baseBranchSha": "22206412ee0bd3b0b08d8769057fb88de273b484",
      "branchName": "renovate/python-3.x",
      "branchSha": "ed82288aaebbe067d366d856c2ec611690e4a94f",
      "isModified": false,
      "isPristine": true
    }
  ],
  "inactiveBranches": []
}
DEBUG: Renovate repository PR statistics
{
  "stats": {
    "total": 1,
    "open": 1,
    "closed": 0,
    "merged": 0
  }
}
DEBUG: Repository result: done, status: onboarded, enabled: true, onboarded: true
DEBUG: Repository timing splits (milliseconds)
{
  "splits": {
    "init": 5631,
    "extract": 2262,
    "lookup": 2703,
    "onboarding": 0,
    "update": 6919
  },
  "total": 19900
}
DEBUG: Package cache statistics
{
  "get": {
    "count": 2,
    "avgMs": 3,
    "medianMs": 1,
    "maxMs": 4
  },
  "set": {
    "count": 0
  }
}
DEBUG: http statistics
{
  "urls": {
    "https://api.github.com/graphql (POST,200)": 3,
    "https://api.github.com/repos/Hongbo-Miao/bug-renovate-python-version/git/commits (POST,201)": 1,
    "https://api.github.com/repos/Hongbo-Miao/bug-renovate-python-version/git/refs (POST,201)": 1,
    "https://api.github.com/repos/Hongbo-Miao/bug-renovate-python-version/git/trees (POST,201)": 1,
    "https://api.github.com/repos/Hongbo-Miao/bug-renovate-python-version/issues (POST,201)": 1,
    "https://api.github.com/repos/Hongbo-Miao/bug-renovate-python-version/pulls (GET,200)": 1,
    "https://api.github.com/repos/Hongbo-Miao/bug-renovate-python-version/pulls (POST,201)": 1,
    "https://api.github.com/repos/whitesource/merge-confidence/contents/beta.json (GET,200)": 1
  },
  "hostStats": {
    "api.github.com": {
      "requestCount": 10,
      "requestAvgMs": 361,
      "queueAvgMs": 0
    }
  },
  "totalRequests": 10
}
DEBUG: dns cache
{
  "hosts": [
    "api.github.com"
  ]
}
INFO: Repository finished
{
  "cloned": true,
  "durationMs": 19900
}
  ```
</details>
