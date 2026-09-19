# ARK-tube

Organization-level repository for **ARK-tube**. It holds the org profile page and, optionally,
default community health files shared by every repository in the org.

This repository contains no application code. The app lives in
[ARK-tube/ARKtube](https://github.com/ARK-tube/ARKtube).

## What's here

```text
.github/
├── README.md            this file (visible only on this repo's page)
└── profile/
    └── README.md        rendered on https://github.com/ARK-tube
```

### `profile/README.md`: the organization profile

GitHub renders this file at the top of the organization's home page. It works only if:

- the repository is named exactly `.github`
- the repository is **public**
- the file is at exactly `profile/README.md`

Edit that file to change what visitors see at `github.com/ARK-tube`. This root README is
**not** shown there.

### Default community health files (optional)

Files placed in this repo are used as fallbacks by any org repository that doesn't have its
own copy. Supported files include:

| File | Purpose |
|---|---|
| `CONTRIBUTING.md` | How to contribute |
| `CODE_OF_CONDUCT.md` | Community standards |
| `SECURITY.md` | How to report vulnerabilities |
| `SUPPORT.md` | Where to get help |
| `ISSUE_TEMPLATE/` | Default issue forms and templates |
| `PULL_REQUEST_TEMPLATE.md` | Default pull request template |

They can sit in the repo root, in `docs/`, or in a `.github/` folder. A repository's own
file always takes precedence over the default from here.

## Related

- [ARKtube](https://github.com/ARK-tube/ARKtube): the native GTK3 + WebKit2GTK client for `youtube.com/tv`

---

<sub>ARKtube is an independent project. It is not affiliated with or endorsed by Google or YouTube.
YouTube is a trademark of Google LLC.</sub>
