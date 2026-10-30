---
layout: page
title: Liu Wentao — Resume
---

## Profile

Front-end engineer with 13+ years of experience (since 2013). Joined ByteDance in 2023.08; since 2023.10, led the front-end of Feishu Contract Web, from core-module development to overall ownership, and led the Web team (10 people, later 4) on work allocation, scheduling and delivery. Strong in React + TypeScript and front-end engineering; led the Webpack → Rspack migration, cutting build time by 80%+ with no production incidents. Experienced in stability engineering and error monitoring for large-scale B2B products, and in Web / mini-program / React Native multi-platform architecture.

## Details

- Name: Liu Wentao (ik0r)
- Open to: Front-end Lead / Senior Front-end Engineer
- Email: jobs@ik0r.com
- Phone: 18501335721
- GitHub: <https://github.com/ik0r>
- Blog: <https://isay.me>

## Work Experience

| Period | Company | Role |
| --- | --- | --- |
| 2023.08 – 2026.07 | ByteDance | Front-end Lead (Level 2-2) |
| 2017.02 – 2023.08 | Meituan (Beijing Sankuai Online Technology Co., Ltd.) | Front-end Engineer (2-1 → 2-2 → 3-1 → L8) |
| 2014.06 – 2017.02 | Beijing Weikuke Technology Co., Ltd. | Front-end Engineer |
| 2013.03 – 2014.05 | AutoNavi Software Co., Ltd. (Amap) | Front-end Engineer (intern 2013.03–2013.07) |

## Project Experience

### ByteDance · Feishu Contract Web, Mini Program and LetSign Platform (2023.10 – 2026.07)

- Overview: Feishu Contract is Feishu's one-stop contract lifecycle management product, covering drafting, online negotiation, review and approval, signing, performance and analytics, serving several leading enterprise customers. Also responsible for the Web front-end of the LetSign (<https://www.letsign.com/>) e-signature platform.
- Responsibilities:
    - As front-end owner of Feishu Contract Web, led the overall front-end effort and drove the architecture and iteration of core modules: online negotiation (China and non-China regions), contract status transitions and approval flows, multi-party signing and sealing/archiving, admin-side process and field management, bulk contract applications, contract ledger, and contract templates. Also developed and maintained the Feishu Contract mini program (Taro) and the LetSign platform Web front-end.
    - Led the Web team (10 people, later 4) on work allocation, scheduling and delivery, while remaining hands-on in core modules.
    - Led the build system migration from Webpack (Jupiter) to Rspack (Edenx), resolved build compatibility issues, cut build time by 80%+, and shipped with no production incidents.
    - For online negotiation, where multiple parties are online simultaneously and events come from many sources, used rxjs Subject and Operators to unify event streams, covering aggregation, dispatch and subscription cleanup, reducing races and state inconsistency across sources.
    - Owned Web stability and error monitoring; participated in the continuous delivery pipeline (automated builds, swimlane environment verification, gradual rollout) and on-call response; integrated and maintained the WPS SDK in Feishu Contract.
    - Gated feature visibility by permission flags issued by the backend and rendered contract-sensitive data according to desensitization results, meeting enterprise customers' access-control and data-security requirements.

### Meituan · Delivery Front-end Architecture and Stability (2017.02 – 2023.08)

- Overview: Owned front-end architecture, build systems and stability for Meituan delivery rider-facing Web, React Native (MRN) and mini-program products, covering architecture iteration and multi-platform integration, as well as log reporting, incident prevention, detection, mitigation and root-cause analysis.
- Responsibilities:
    - **Web and MRN architecture** (2017.02 – 2023.08): Owned the architecture and build system for all H5 and some admin pages, using a monorepo and per-directory/per-page deployments; led the MRN architecture upgrade, collecting developer pain points and fixing them at the framework level, while also building business pages; drove the upgrade and migration of the rider app's Hybrid Web container (KNB); built a unified scaffolding tool for Web, MRN and mini-program projects based on @angular-devkit/schematics.
    - **Front-end stability program** (2018.03 – 2023.08): Upgraded mini-program, Web and MRN architectures with error, API and log reporting; defined stability development standards with checkpoints at key stages, and built front-end failure playbooks for each page; defined stability metrics and tuned alerting policies; documented troubleshooting practices and promoted log-query tooling (SQL, Presto, Hive, Kibana) across the team.
    - **Rider mini-program architecture** (2020.04 – 2023.08): Built the delivery-locker mini program from 0 to 1, defining its architecture, processes and development standards; designed and implemented a multi-app monorepo architecture using Rollup, Gulp, ESLint, TypeScript and in-house tooling, enabling code sharing and reuse across 4 mini programs (delivery lockers, battery-swap lockers and their operations apps); drove the rider app's adoption of the Meituan mini-program SDK, unifying the delivery-locker app from a "mini program + React Native" stack to a single mini-program stack and integrating it into Meituan Crowdsourcing and Meituan Dedicated Delivery.
    - **Map migration adapter library** (2017.08 – 2018.05): During the company-wide move away from Amap, built an adapter that let business code migrate from the Amap JS SDK to Tencent Maps with minimal changes while supporting multiple map providers; researched API, feature and coordinate-system differences across Amap, Tencent, Baidu and Google Maps; designed and implemented a seed → loader → lib layered adapter architecture with map selection and automatic fallback; coordinated the department-wide Web migration from Amap to Tencent Maps.

### Early Projects (2013.03 – 2017.01)

- **WeCook grocery assistant** (2014.11 – 2017.01): Web and WeChat platform products "Weiwei Gourmet / Maicai Bangshou / WeCook Seafood", helping users buy fresh semi-prepared food. Built the front-end architecture and tech selection on AngularJS; set up the full build system, evolving from source publishing → Grunt → Gulp → Webpack → FIS3; established commit conventions; delivered most of the front-end and part of the back-end.
- **Lightweight visual page editor (Taobao Magic Pen-like, internal experiment at WeCook)** (2016.01 – 2016.06): A WYSIWYG content editor, similar to a simplified PowerPoint, supporting drag and resize to help operations teams quickly generate campaign and product pages, with structured output for reuse across platforms. Owned front-end architecture and tech selection, build system setup, reusable component abstraction, and front-end/back-end data contracts.
- **Amap Web and mobile products** (2013.03 – 2014.05): Worked on Amap PC POI detail pages, the mobile Web SPA, AMap JS API 2.0 and the front-end vector map. Owned tech selection and architecture for the mobile Web SPA from 0 to 1, ensuring URL re-entrancy across single-page states; contributed to AMap JS API 2.0, building overlays such as Marker, InfoWindow and context menu, and extracted a reusable library based on Google Maps' MVCObject pattern; explored HTML5 Canvas-based vector map tile rendering and performance optimization.

## Technical Writing

- "TypeScript Type Challenges" — internal tech talk. Systematically covered conditional types, mapped types, recursive types, keyof, extends constraints and infer, to build team TypeScript expertise.
- "Learning RxJS with Feishu Contract" — internal tech talk. Walked through Observable, Subject, Scheduler and common Operators as used in the actual codebase, lowering the team's cost of understanding and maintaining rxjs code.

## Skills

- **Front-end architecture and leadership**: Led complete architecture and tech selection for complex Web, mini-program and React Native projects; monorepo experience; led work allocation, scheduling and delivery for a 10-person team while staying hands-on in core modules.
- **Stack**: React + TypeScript as primary; familiar with Vue, React Native and Taro; zustand for state, react-query / swr for server state, styled-components for styling; multilingual support for China and non-China regions via a copy-management platform and react-i18n.
- **Engineering and build**: Webpack, Rspack and Edenx (open-source counterpart: Modern.js); led build system setup across multiple projects and completed the Webpack → Rspack migration.
- **Type system**: Deep familiarity with TypeScript's type system and type-level programming; added type definitions to most libraries I maintain.
- **Reactive programming**: Experienced with rxjs; used Observable, Subject, Scheduler and Operators to handle asynchronous event streams in large projects.
- **Stability**: Built stability practices across multiple projects, covering error monitoring, log reporting, alerting and troubleshooting.
- **Other**: WeChat official accounts and Hybrid App (JSBridge); Amap, Tencent, Baidu and Google Maps SDKs; Node.js (Express, Koa, MongoDB); CSS2/CSS3, SASS/LESS, PostCSS; Karma and Mocha; Git with GitHub workflow and gitflow.

## Other Skills

- Linux and macOS user since 2009 (*nix: Debian, Ubuntu, Fedora, CentOS, Gentoo), comfortable with directory structure, permissions and configuration; Docker, docker-compose, nginx and Traefik.
- Early PHP experience: built 3 WordPress themes; familiar with ThinkPHP.

## Education

- 2009 – 2013 · Ocean University of China · Communication Engineering
- English: CET-6
