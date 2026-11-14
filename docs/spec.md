# GOV.UK Service Manual — Testing your service — throughline source

This document is **generated from the graph** by `tl docs`; `tl docs --check` gates it in
CI. The prose headings are hand-owned — everything between `tl:*` markers is injected from
the YAML items, so the published spec can never drift from the graph.

This source expresses the GOV.UK Service Manual **"Testing your service"** guidance: each
Service Manual page is a `user_requirement`, and each guidance point is a
`system_requirement` that `implements` its page. The page lives in `attrs.source_ref`. The
throughline UIDs are this source's own and immutable — a consumer cites a point as
`govuktesting:SR-0003`, never by a page name.

Contains
<!-- tl:count type == 'user_requirement' -->
6
<!-- tl:end --> pages and
<!-- tl:count type == 'system_requirement' -->
47
<!-- tl:end --> guidance points.

GOV.UK Service Manual content is © Crown copyright, reused here under the Open Government
Licence v3.0. See `NOTICE`.

## Purpose

<!-- tl:item INT-0001 -->
**INT-0001 — A government service is tested continuously across quality, security, performance and accessibility** — `intent`, status `proposed`

> The GOV.UK Service Manual 'Testing your service' guidance exists so that a public digital service is tested continuously and holistically — quality assurance, exploratory, security, performance and accessibility testing — throughout its lifecycle, so it works well and safely for all users before and after it goes live.

**source_ref**: GOV.UK Service Manual — Testing your service
<!-- tl:end -->

## Quality assurance: testing your service regularly

<!-- tl:item UR-0001 -->
**UR-0001 — Quality assurance: testing your service regularly** — `user_requirement`, status `proposed`

> Make quality everyone's responsibility and test the service regularly, in realistic conditions, using a range of automated and manual test types.

*Derives from:* INT-0001

**source_ref**: GOV.UK Service Manual — Quality assurance: testing your service regularly · **url**: https://www.gov.uk/service-manual/technology/quality-assurance-testing-your-service-regularly
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'GOV.UK Service Manual — Quality assurance: testing your service regularly' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0001 | system_requirement | proposed | Make quality a whole-team responsibility |
| SR-0002 | system_requirement | proposed | Test in realistic conditions |
| SR-0003 | system_requirement | proposed | Automate tests on every change |
| SR-0004 | system_requirement | proposed | Review your testing approach regularly |
| SR-0005 | system_requirement | proposed | Use a range of test types |
| SR-0006 | system_requirement | proposed | Bring in external expertise where needed |
| SR-0007 | system_requirement | proposed | Test accessibility from beta onward |
| SR-0008 | system_requirement | proposed | Get fast feedback to catch issues early |
<!-- tl:end -->

## Exploratory testing

<!-- tl:item UR-0002 -->
**UR-0002 — Exploratory testing** — `user_requirement`, status `proposed`

> Use unscripted, goal-directed exploration to find defects that scripted tests miss, capturing evidence and feeding findings back into automation.

*Derives from:* INT-0001

**source_ref**: GOV.UK Service Manual — Exploratory testing · **url**: https://www.gov.uk/service-manual/technology/exploratory-testing
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'GOV.UK Service Manual — Exploratory testing' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0009 | system_requirement | proposed | Set a clear goal for each session |
| SR-0010 | system_requirement | proposed | Time-box exploratory sessions |
| SR-0011 | system_requirement | proposed | Use test charters |
| SR-0012 | system_requirement | proposed | Capture evidence |
| SR-0013 | system_requirement | proposed | Record ideas for further testing |
| SR-0014 | system_requirement | proposed | Automate issues found during exploration |
<!-- tl:end -->

## Vulnerability and penetration testing

<!-- tl:item UR-0003 -->
**UR-0003 — Vulnerability and penetration testing** — `user_requirement`, status `proposed`

> Regularly assess the whole system's security using appropriately certified testers and automated tooling, with proper consent, agreements and handling of reports.

*Derives from:* INT-0001

**source_ref**: GOV.UK Service Manual — Vulnerability and penetration testing · **url**: https://www.gov.uk/service-manual/technology/vulnerability-and-penetration-testing
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'GOV.UK Service Manual — Vulnerability and penetration testing' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0015 | system_requirement | proposed | Assess security regularly, especially on major changes |
| SR-0016 | system_requirement | proposed | Scope testing to the whole system |
| SR-0017 | system_requirement | proposed | Get consent from third-party suppliers |
| SR-0018 | system_requirement | proposed | Use appropriately certified testers |
| SR-0019 | system_requirement | proposed | Agree scope, timing and liability in contracts |
| SR-0020 | system_requirement | proposed | Handle test reports securely |
| SR-0021 | system_requirement | proposed | Build internal security capability |
| SR-0022 | system_requirement | proposed | Automate vulnerability detection |
<!-- tl:end -->

## Test your service's performance

<!-- tl:item UR-0004 -->
**UR-0004 — Test your service's performance** — `user_requirement`, status `proposed`

> Plan for expected load, then load- and stress-test the service to find its limits and make an informed decision about acceptable risk before going live.

*Derives from:* INT-0001

**source_ref**: GOV.UK Service Manual — Test your service's performance · **url**: https://www.gov.uk/service-manual/technology/test-your-services-performance
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == "GOV.UK Service Manual — Test your service's performance" -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0023 | system_requirement | proposed | Do capacity planning first |
| SR-0024 | system_requirement | proposed | Run load tests against pre-production |
| SR-0025 | system_requirement | proposed | Test beyond expected limits |
| SR-0026 | system_requirement | proposed | Increase load gradually until failure |
| SR-0027 | system_requirement | proposed | Record the failure point and degradation |
| SR-0028 | system_requirement | proposed | Have the service owner assess acceptable risk |
| SR-0029 | system_requirement | proposed | Optimise under stress |
| SR-0030 | system_requirement | proposed | Monitor performance trends over time |
<!-- tl:end -->

## Testing with assistive technologies

<!-- tl:item UR-0005 -->
**UR-0005 — Testing with assistive technologies** — `user_requirement`, status `proposed`

> Test the service continuously with the required assistive technologies and browser combinations so it works for disabled users.

*Derives from:* INT-0001

**source_ref**: GOV.UK Service Manual — Testing with assistive technologies · **url**: https://www.gov.uk/service-manual/technology/testing-with-assistive-technologies
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'GOV.UK Service Manual — Testing with assistive technologies' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0031 | system_requirement | proposed | Test the required assistive-technology combinations |
| SR-0032 | system_requirement | proposed | Test continuously during development |
| SR-0033 | system_requirement | proposed | Use real devices where possible |
| SR-0034 | system_requirement | proposed | Verify screen-reader access to every element |
| SR-0035 | system_requirement | proposed | Test magnification layout and spacing |
| SR-0036 | system_requirement | proposed | Test speech recognition with natural speech |
| SR-0037 | system_requirement | proposed | Document accessibility issues with environment detail |
| SR-0038 | system_requirement | proposed | Prioritise barriers by severity |
| SR-0039 | system_requirement | proposed | Include assistive-technology users in research |
<!-- tl:end -->

## How to test frontend performance

<!-- tl:item UR-0006 -->
**UR-0006 — How to test frontend performance** — `user_requirement`, status `proposed`

> Treat frontend performance as a first-class concern: set a budget, benchmark, test across devices and integrate performance checks into releases.

*Derives from:* INT-0001

**source_ref**: GOV.UK Service Manual — How to test frontend performance · **url**: https://www.gov.uk/service-manual/technology/how-to-test-frontend-performance
<!-- tl:end -->

<!-- tl:table type == 'system_requirement' and attrs.get('source_ref') == 'GOV.UK Service Manual — How to test frontend performance' -->
| UID | Type | Status | Title |
|---|---|---|---|
| SR-0040 | system_requirement | proposed | Include frontend performance in service documentation |
| SR-0041 | system_requirement | proposed | Prototype and design in the browser early |
| SR-0042 | system_requirement | proposed | Test across a wide range of devices |
| SR-0043 | system_requirement | proposed | Set and enforce a performance budget |
| SR-0044 | system_requirement | proposed | Benchmark with standard tools |
| SR-0045 | system_requirement | proposed | Optimise identified bottlenecks |
| SR-0046 | system_requirement | proposed | Measure before-and-after impact |
| SR-0047 | system_requirement | proposed | Integrate performance checks into releases |
<!-- tl:end -->
