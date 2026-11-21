# Design and product skills

A field guide for product managers, designers, and engineers working on the same feature. Use it to choose a skill for the decision in front of you, from the first research question to a tested interaction on a phone.

**Example:** A team sees people abandon onboarding. Start with **metrics-review** to locate the drop, then use **user-research** to investigate it. Challenge the proposed fix with **grill-me**, compare two flows with **prototype**, and use **design-handoff** to specify error, loading, and recovery states. Revisit the original metric after release.

[Plugins and installation](#plugins-and-installation) · [Mobile and author collections](#mobile-and-author-collections) · [Product discovery](#product-discovery-and-delivery) · [Interface design](#interface-design-and-prototyping) · [Figma](#figma) · [Motion](#motion-and-video) · [Design systems](#design-systems-and-visual-design)

## Plugins and installation

This repository publishes three installable Claude Code marketplace entries. Each points to its publisher at a pinned revision. Add the marketplace once, then install the plugins you want in Claude Code:

```text
/plugin marketplace add arthurhux/design-product-skills
/plugin install design@design-product-skills
/plugin install product-management@design-product-skills
/plugin install engineering@design-product-skills
```

| Plugin or integration | When to use it | Where to get it |
|---|---|---|
| Design | Review a flow, audit accessibility, and prepare component specs for handoff. | This marketplace · [Anthropic](https://github.com/anthropics/knowledge-work-plugins/tree/main/design) |
| Product Management | Connect research findings to a spec, roadmap decision, and success metric. | This marketplace · [Anthropic](https://github.com/anthropics/knowledge-work-plugins/tree/main/product-management) |
| Engineering | Turn a design decision into a technical plan and review the implementation. | This marketplace · [Anthropic](https://github.com/anthropics/knowledge-work-plugins/tree/main/engineering) |
| Figma | Work with editable frames, components, and design-to-code mappings. | [Figma developer tools](https://developers.figma.com/) |
| Mobbin | Compare a proposed flow with screenshots from shipped products. | [Mobbin](https://mobbin.com/) |
| Market Researcher | Investigate a market before committing to discovery or positioning work. | Host-provided plugin, listed as Market Researcher where available |
| Firecrawl | Gather public product pages and documentation for a competitive brief. | [Firecrawl](https://github.com/firecrawl/firecrawl-mcp-server) |
| ElevenLabs | Create voiceovers for a walkthrough and test the pacing against the prototype. | [ElevenLabs](https://github.com/elevenlabs/elevenlabs-mcp) |
| Sites | Turn an approved brief into a working landing page or internal tool. | Host-provided Sites integration where available |
| Remotion | Render a repeatable video composition from React, such as a demo with changing product data. | [Publisher's skills](https://github.com/remotion-dev/skills) |
| HyperFrames | Build an HTML-based video or port an existing motion composition. | [Publisher's skills](https://github.com/heygen-com/hyperframes) |

Connected tools use the host's account and workspace permissions. In the catalog below, linked skill names lead to their source collections. Plain names identify workflows from the inventory whose individual public distribution links have yet to be confirmed.

## Mobile and author collections

The repository includes pinned Git submodules for **Android**, **SwiftUI**, and **Emil Kowalski**. To fetch their skill files along with the guide:

```sh
git clone --recurse-submodules https://github.com/arthurhux/design-product-skills.git
```

For an existing clone, run `git submodule update --init --recursive`. Each collection includes its own setup instructions and license information.

| Collection | What to reach for first |
|---|---|
| [Android skills by Google](collections/android) | For a screen migration, start with XML Views to Compose. For tablets and foldables, use adaptive layouts. For content obscured by system bars, use edge-to-edge. The collection also covers navigation, testing, and performance. |
| [SwiftUI Expert by Antoine van der Lee](collections/ios) | Use **swiftui-expert-skill** to review how a screen owns state, composes views, and updates during scrolling. |
| [Emil Kowalski's skills](collections/emil) | Use **break-ui** to stress a layout with difficult content, **gestures** for direct manipulation, **choreograph** for coordinated transitions, and **remove-animations** to simplify distracting motion. |
| [Interface Craft by Josh Puckett](https://www.interfacecraft.dev/) | Use **interface-craft** to storyboard an interaction, tune its timing, and critique the result. Josh distributes the skill files through his membership. His public [DialKit library](https://github.com/joshpuckett/dialkit) provides live controls for comparing values in a running interface. |

**Browse the individual bundled skills:** [Android, iOS, and Emil Kowalski index](COLLECTIONS.md).


## Interface design and prototyping

| Skill | When to use it |
|---|---|
| [apple-design](https://github.com/emilkowalski/skills) | Review a swipe, drag, or sheet on the web when its movement should follow the user's finger. |
| ckm:design | Carry one visual identity across logos, tokens, interface styling, and presentation assets. |
| ckm:ui-styling | Compose accessible controls with shadcn/ui and Tailwind when implementing a screen. |
| creative-studio | Generate voice, music, or other media through ElevenLabs for a narrated prototype. |
| design | Extract a site's typography, tokens, and component conventions into a reusable DESIGN.md. |
| design-critique | Review a mockup before handoff to find unclear hierarchy, inconsistent controls, or friction. |
| design-handoff | Specify component states, breakpoints, and tokens so engineering can implement a design. |
| [emil-design-eng](https://github.com/emilkowalski/skills) | Review the details of feedback, timing, and component behavior in a working interface. |
| [excalidraw-diagram](https://github.com/coleam00/excalidraw-diagram-skill) | Draw an editable workflow diagram when a sequence of handoffs is hard to explain in prose. |
| [frontend-design](https://github.com/anthropics/claude-code) | Build a web interface around a deliberate type, layout, and visual direction. |
| [pick-ui-library](https://github.com/emilkowalski/skills) | Choose a library for a specific interaction such as a command menu or draggable list. |
| [prototype](https://github.com/emilkowalski/skills) | Build alternative versions of one interaction and compare them in a live picker. |
| redesign-screen | Compare a screen with shipped examples from Mobbin before choosing a redesign direction. |
| swiftui-liquid-glass | Review material, layering, and readability when adopting Liquid Glass in SwiftUI. |
| swiftui-performance-audit | Investigate slow scrolling or excessive view updates before choosing what to profile. |
| swiftui-ui-patterns | Choose SwiftUI navigation, state, and layout patterns while composing a screen. |
| swiftui-view-refactor | Split a large SwiftUI view and clarify state ownership so changes stay testable. |
| ui-ux-pro-max | Explore palettes, type pairings, and interface patterns for a web or mobile brief. |
| uiux-design-consultant | Work through wireframes and interaction choices when the user flow is still unsettled. |
| ux-copy | Write a label, error, or empty state that tells the reader what they can do next. |
| ux-researcher | Plan usability testing to check whether people can complete a proposed flow. |

## Figma

| Skill | When to use it |
|---|---|
| figma-3d-transforms | Add perspective or depth when a flat rotation cannot express the intended effect. |
| figma-code-connect | Map a library component to its production code example so developers can reuse it. |
| figma-code-workflows | Bring HTML or a project into Figma as editable frames or a runnable code layer. |
| figma-create-new-file | Start a Design, FigJam, or Slides file in the right workspace for a new deliverable. |
| figma-design-to-code | Translate a selected frame into application code using its design context. |
| figma-generate-design | Reconstruct an application screen in Figma so the team can edit its layout. |
| figma-generate-diagram | Turn a process or architecture into a diagram colleagues can review together. |
| figma-generate-library | Build variables, components, and variants from a codebase to create a shared library. |
| figma-generative-plugins | Package a repeatable generative operation as a reusable Figma plugin. |
| figma-implement-motion | Translate timing and easing from a motion design into application code. |
| figma-preflight | Check the connection, available libraries, and tokens before editing a shared file. |
| figma-shaders | Create a custom shader fill when a static color or gradient cannot produce the effect. |
| figma-spec | Write and review a brief or specification alongside the design it describes. |
| figma-style-binding | Bind spacing, color, and text to shared variables and styles so changes propagate. |
| figma-swiftui | Move between SwiftUI views and Figma when checking a native implementation against its design. |
| figma-use | Read or edit canvas nodes through the Figma bridge for precise changes to a file. |
| figma-use-figjam | Arrange flows and workshop material on a collaborative FigJam board. |
| figma-use-motion | Set keyframes, duration, and easing to preview an interaction directly in Figma. |
| figma-use-slides | Build and edit a slide deck within the Figma Slides workspace. |

## Motion and video

| Skill | When to use it |
|---|---|
| [animate](https://github.com/emilkowalski/skills) | Choose the property, curve, and duration for a new web interaction. |
| [animate-expo](https://github.com/emilkowalski/skills) | Build a responsive gesture or transition for React Native and Expo. |
| [animation-performance](https://github.com/emilkowalski/skills) | Diagnose dropped frames and choose less expensive properties or rendering work. |
| [animation-vocabulary](https://github.com/emilkowalski/skills) | Find the precise term for a motion effect before describing it to a collaborator. |
| [find-animation-opportunities](https://github.com/emilkowalski/skills) | Identify interactions where motion would explain a change and propose specific timings. |
| [improve-animations](https://github.com/emilkowalski/skills) | Prioritize motion issues across an existing codebase and prepare implementation plans. |
| [remotion-best-practices](https://github.com/remotion-dev/skills) | Find the relevant Remotion guidance when producing a repeatable, code-driven video. |
| [review-animations](https://github.com/emilkowalski/skills) | Review an implemented animation for timing, responsiveness, and consistency. |

## Product discovery and delivery

| Skill | When to use it |
|---|---|
| competitive-analysis | Map the competitive landscape when preparing a positioning or strategy deck. |
| competitive-brief | Compare a focused feature area to inform a specific product decision. |
| grill-me | Stress-test a proposal one question at a time before committing to its assumptions. |
| grill-with-docs | Challenge a proposal against the project's vocabulary and record decisions as they settle. |
| metrics-review | Investigate changes in product metrics and decide what to examine next. |
| product-brainstorming | Explore possible solutions while the underlying customer problem is still open. |
| research-synthesis | Combine interviews, support tickets, and usability observations into themes for design review. |
| roadmap-update | Reprioritize initiatives and make the consequences for existing commitments visible. |
| sprint-planning | Scope a sprint against team capacity and agree on a goal the team can deliver. |
| stakeholder-update | Explain progress, risks, and decisions at the level a particular audience needs. |
| synthesize-research | Turn a batch of feedback into evidence-backed insights for product planning. |
| user-research | Plan an interview, survey, or usability study around a specific research question. |
| write-spec | Convert an idea into a feature spec with scope, success criteria, and open questions. |

## Design systems and visual design

| Skill | When to use it |
|---|---|
| accessibility-review | Audit a page or design for barriers such as missing focus indicators and low contrast. |
| [better-accessibility](https://github.com/jakubkrehel/skills) | Fix keyboard, screen-reader, zoom, and reduced-motion behavior in an implementation. |
| [better-colors](https://github.com/jakubkrehel/skills) | Define semantic color tokens and check contrast across a palette. |
| [better-interface](https://github.com/jakubkrehel/skills) | Review layout, writing, color, accessibility, and polish together before release. |
| [better-layout](https://github.com/jakubkrehel/skills) | Check grouping and reading order under resizing, translation, and mirrored layouts. |
| [better-typography](https://github.com/jakubkrehel/skills) | Review type scale, wrapping, and truncation against real interface content. |
| [better-ui](https://github.com/jakubkrehel/skills) | Refine icon alignment, surface borders, shadows, and control states. |
| [better-writing](https://github.com/jakubkrehel/skills) | Make labels, confirmations, and recovery instructions consistent with the product voice. |
| brand-identity | Collect an organization's existing visual identity before preparing branded material. |
| ckm:banner-design | Develop banner and hero variants for different placements and aspect ratios. |
| ckm:brand | Define voice, messaging, and asset rules for consistent branded content. |
| ckm:design-system | Connect primitive, semantic, and component tokens to implementation specifications. |
| design-system | Audit existing components for naming drift, missing states, and undocumented variants. |
| graphic-design-fundamentals | Use composition, color, and typography to clarify the message of a visual. |
| pixijs-accessibility | Add keyboard and screen-reader access to a PixiJS canvas interface. |
| presentation-design-expert | Structure slides and charts so an audience can follow the argument. |
