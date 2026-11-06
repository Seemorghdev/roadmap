# Mehridian roadmap

An evidence-linked index of what the projects have shown, what is being worked on, and the questions they leave open.

**Status.** Built: a public roadmap for four site projects. Evidence: all four project links were checked against the live site on 6 November 2026. Limits: roadmap stages describe evidence and current work; an open question is not a commitment.

## Verify

Requirement: `curl` with network access.

```bash
for url in \
  https://mehridian.tech/projects/small-object-detection \
  https://mehridian.tech/projects/seemorgh-operator-console \
  https://mehridian.tech/projects/edge-evidence \
  https://mehridian.tech/research/project03; do
  curl -sS -L -o /dev/null -w '%{http_code} %{url_effective}\n' "$url"
done
```

Expected: four final `200` responses. Project 03 currently redirects to its slash-terminated route.

## Tests

No automated test suite or GitHub Actions workflow is configured in this repository. The Verify command above checks the four live project links.

## How it fits

This is the evidence index for [Mehridian](https://mehridian.tech). The public board is at https://github.com/users/Seemorghdev/projects/2.

### Three words

- **Shown:** a result a published page or public record shows. Every Shown item links its evidence.
- **Working on:** in motion now.
- **Open question:** a question a published page names as open. **Not a commitment.**

### The projects

| Project | Field | Page |
| --- | --- | --- |
| Small Objects in Big Frames | Perception | https://mehridian.tech/projects/small-object-detection |
| Seemorgh operator console | Sensor fusion | https://mehridian.tech/projects/seemorgh-operator-console |
| Edge Evidence | Data integrity | https://mehridian.tech/projects/edge-evidence |
| Project 03 | Engineering audit | https://mehridian.tech/research/project03 |
| Linguistic Pipeline | Language | Overview coming |

### How items change

- When a Working on item is published, it becomes Shown, with its link.
- An Open question nobody pursues gets the note "not planned"; it isn't silently removed.
- Nothing here refers to private work.

## Licence

CC BY 4.0. See `LICENSE`.
