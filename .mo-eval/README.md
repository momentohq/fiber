# Why this fork exists

An organisation-owned fork of `gofiber/fiber`, so mo-eval has a second Go benchmark alongside gin and
so results are visible to the whole organisation — access is scoped by a repository's owner.

Chosen on two measurements, after an earlier attempt on a mature library selected zero tasks:
300 merged pull requests reach back only inside the 400-day window, and 14 of 30 recent ones touch
non-test source. Recency alone is not fit.

Go rather than another language because Go is currently the only language with a built-in
`offline_prepare` (`go mod vendor`); the others need the repository to supply one and there is no
worked example, so their bundles do not ship.
