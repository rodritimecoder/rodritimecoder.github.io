# Align · the terminal notebook

A lightweight `apiv-loop` align artifact. This is the *What / What NOT* pass that
happened before any code was written. It is intentionally short: a blog does not
need the full align → plan → dispatch → verify ceremony.

## What

- A single-author blog served by GitHub Pages, built by Jekyll with no custom CI.
- Home page with the latest three posts, a full post index with counts, and one
  real sample post to prove the template.
- Dressed in the `glitch-console` look from `design-pack`: dark terminal, six
  primitives only, every colour from `tokens.css`.
- Two observable gates on the rendered site: `design-pack verify` (static token
  conformance) and `design-pack check` (runtime behaviour across seven viewports).

## What NOT

- No CMS, no comments, no newsletter, no analytics.
- No web controls inside the terminal windows — navigation is links and `.line`s.
- No new design look. `glitch-console` is the only look in the pack; a new one is
  a separate project.
- No remote yet. The repo is local until the first version is verified.
- No full APIV dispatch/verify scaffolding. The gates above are the evidence;
  APIV's `verify` only records that a verification happened.

## References

- `design-pack` — `omnicli describe design-pack` (Quick use, Use the pack, gates).
- `apiv-loop` — `omnicli describe apiv-loop` (the 4-phase loop, Fail → align).
- Look contract: `design-pack/looks/glitch-console/tokens.css` and `README.md`.

## Escalation trigger

If this grows into a multi-feature or multi-author project, move to the full
APIV loop, or BMAD if several people need to agree on requirements up front.
