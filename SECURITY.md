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
