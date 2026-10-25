# Working on this site

This repository was created and is published by Yard Crew's trusted delivery
code. People and agents who change it follow the same rules.

- **The tests are the acceptance contract.** `tests/` and `.github/` belong to
  the owner (CODEOWNERS). Never edit them to make a change pass.
- **Test first.** Run `python -m unittest discover -s tests` before and after a
  change, and keep the pre-commit hooks installed (`pre-commit install`).
- **Static only.** Everything in `site/` is public. No scripts, keys, trackers
  or server code. Use `%BASE%` for local links so the site works under its path.
- **Accessible by default.** One `h1`, header, main and footer landmarks, alt
  text, visible focus, sufficient contrast, reduced-motion support.
- **Clean up after yourself.** Keep files small and the repository lean: no
  build output, caches or large binaries in Git; CI keeps no artifacts.
- **Evidence over claims.** A change is done when the tests pass and the
  published page shows its release marker, not when it looks finished.
- **Nothing here decides payment, release or authority.** Publication is done
  by the trusted delivery process, which verifies the live site.
