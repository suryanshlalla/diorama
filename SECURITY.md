# Security policy

## Scope

The published website is static and runs a client-side Three.js app; it has no
first-party public application server or private credentials. The repository
also contains an opt-in local About editor server used only by `npm run
dev:edit`. It binds to loopback and accepts validated document saves to
`content/laptop/about.json`. Do not expose that development server to an
untrusted network. The published site is built from this repository and
deployed to the `main` branch of `suryanshlalla/diorama` by
`tools/publish-pages.sh --publish`.

Third-party services currently used by the app include FormSubmit for note
delivery and YouTube for selected music playback. Reports about those services
should go to their operators.

## Reporting a vulnerability

Please report security issues privately to <suryanshlalla10@gmail.com>, the
public contact address configured for the site's note form. Include the
affected URL or file, steps to reproduce, and impact. Please do not include
other people's private submissions or publish an unpatched issue before
contacting the maintainer.

There is no stated response-time or remediation guarantee. This policy does
not promise a security audit or that every issue will be fixed.

## Repository protections

On 2026-09-27, Dependabot vulnerability alerts and automated security updates
were enabled and verified for both the private source repository and the public
Pages repository. The public repository also has secret scanning and secret
push protection enabled. The private repository’s API response did not expose secret-scanning settings;
those features are not claimed as enabled there.

`.github/workflows/checks.yml` validates app/content changes with unit tests,
a dependency audit (including development dependencies), and a production build.
Its token has read-only contents permission, checkout does not retain credentials,
and both official actions are pinned to full commit hashes. The workflow does not
run privileged pull-request code or have access to deployment credentials.

These checks help find regressions and reported dependency vulnerabilities; they
do not verify third-party inbox delivery, prove media redistribution rights, or
guarantee that the application has no vulnerabilities.
