# Ohmbo services

Source: [Ohmbo](https://ohmbo.com/), [how it works](https://ohmbo.com/how-it-works), [pricing](https://ohmbo.com/pricing), [MCP](https://ohmbo.com/docs/mcp), [Developer API](https://ohmbo.com/docs/api). Snapshot reviewed 2026-10-29; check live pages for changing offers.

Ohmbo is a one-stop hardware development platform for the whole hardware journey: requirements and architecture, electronics (schematic, layout and routing), firmware, simulation, 3D structure, appearance and enclosure, engineering changes, prototypes and measured test. Every stage shares one project context, revision history and engineering evidence, and a team can enter at any stage. The website workspace is where the full project, visual inspection, results and commercial workflow live.

Starting points: describe what you want to make and start a project in the workspace; continue from an existing schematic or design; or submit existing design files or requirements for a project review and a design and prototyping quote.

Through the hosted MCP, an agent starts and follows Ohmbo design work with the user's website account: create a design from a plain-language description, revise it, check job status, list jobs, cancel, discover capabilities and retrieve artifact metadata. Jobs run asynchronously and appear under Agent designs on the website, where the complete record and released results are shown. Developer API v1 exposes the native `/v1/designs` contract plus the tested `/v1/models`, `/v1/responses` and `/v1/chat/completions` adapters. Describe this as **Compatible with OpenAI SDKs**. Do not broaden it to every OpenAI parameter, model or synchronous chat behavior.

Plans: anyone can start with Free, with no subscription and one-time trial work credits. Starter, Pro, Business and custom plans add monthly work credits, seats and capacity; the pricing page lists what each plan includes. Prototyping and manufacturing are quoted separately, and downloadable files are released under the published order conditions. Check the pricing page rather than assuming plans, prices or availability remain unchanged.

Evidence: design demonstrations are not proof of physical testing. Automated checks and simulation do not establish engineer approval or physical test results; review, simulation and physical testing each keep their own results on the project.

Scope: the workflow page lists what Ohmbo does not build, including mains-powered (AC) circuits; medical, automotive and aerospace designs; RF design (pre-certified modules are suggested instead); high-speed signals such as USB 3.0+, PCIe and HDMI; rigid-flex or metal-core PCBs; more than 6 layers; and boards over 100 × 100 mm. Refer such requests to the published scope rather than promising acceptance.
