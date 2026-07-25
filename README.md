# throughline-govuk-testing — GOV.UK Service Manual testing guidance as a throughline source

A **throughline source**: a standalone, composable requirements graph that expresses the
GOV.UK Service Manual **"Testing your service"** guidance. A consuming project imports it
under a namespace and references a guidance point by UID:

```toml
# throughline.toml in a consuming project
[[sources]]
namespace = "govuktesting"
url = "https://github.com/rhodium-org/throughline-govuk-testing"
ref = "v2026-07"
```

```yaml
links:
  - target: "govuktesting:SR-0003"   # Automate tests on every change
    type: satisfies
```

It lets a team building a public service ground its test approach in the recognised
government guidance: "our approach *satisfies* `govuktesting:SR-0031` (test the required
assistive-technology combinations)", and so on — checked structurally by
`tl-compose check --strict`.

## Shape

One root intent → 6 Service Manual page `user_requirement`s → 47 guidance-point
`system_requirement`s.

| Page (`user_requirement`) | Points |
|---|---|
| Quality assurance: testing your service regularly | whole-team quality, realistic conditions, automation, review, range of test types, external expertise, accessibility from beta, fast feedback |
| Exploratory testing | session goals, timeboxing, charters, evidence, ideas, automate findings |
| Vulnerability and penetration testing | regular assessment, whole-system scope, third-party consent, certified testers, agreements, report handling, internal capability, automated detection |
| Test your service's performance | capacity planning, load tests, testing beyond limits, ramp to failure, record failure, owner risk decision, optimise under stress, trend monitoring |
| Testing with assistive technologies | required AT/browser combos, continuous testing, real devices, screen-reader coverage, magnification, speech recognition, documentation, severity, real users |
| How to test frontend performance | documented ownership, in-browser early, device range, performance budget, benchmarking, optimisation, before/after measurement, release integration |

The full generated spec is [`docs/spec.md`](docs/spec.md).

## Licence

Apache-2.0 for this repository's structure and tooling — see [`LICENSE`](LICENSE). The GOV.UK
Service Manual content reused here is © Crown copyright, licensed under the
[Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/);
see [`NOTICE`](NOTICE). Each item's `attrs.source_ref` names the Service Manual page it comes
from; the authoritative pages are at
[gov.uk/service-manual/technology](https://www.gov.uk/service-manual/technology). Not
endorsed by or affiliated with GDS or the Crown.

## Editions

The guidance evolves; this cut is tagged `v2026-07`. A later refresh becomes a new tag on
`main`, selected by git `ref`.
