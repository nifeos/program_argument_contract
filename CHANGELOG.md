# Changelog

Dates are UTC. One line per release, what changed and why, so a reader of the diff has the
sentence beside it.

## Unreleased

- First version.
- Removed `PageBuilder::argument_count`. Nothing outside the crate's own tests called it, and a caller that wants the count already has it from `finish`, or reads it from `ArgumentPage::len` after parsing. An item removed before the first release costs no user, while one removed after it would break users.

## BUGS

- The template's lag check guards the CI pin, not this file; a change that matters to a user of
  the crate belongs in a release line here.
