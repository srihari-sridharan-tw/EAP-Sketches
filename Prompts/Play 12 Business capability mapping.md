Generate a colorful sketchnote for the content below, make it colorful and ensure spellings are correct. Aspect Ratio 3:4. I need the background color to be white with no background surface or sketch pens around.

Play #12

# Business capability mapping

Capability Mapping creates a shared understanding of what the organization does (its capabilities) and how those capabilities enable strategy and outcomes. It helps teams move the conversation from systems and structures to business abilities, revealing strengths, gaps, overlaps, and opportunities for reuse or investment. It describes your operating model in terms of goals and competencies (the what) rather than implementation details (the how or by whom).

A Capability Map helps you answer the fundamental questions:
What does the business have to be able to do to execute its strategy? 
How good are we at delivering these capabilities?
Where should we invest to achieve our future state?
Capability models provide a description of the business context that is stable enough to serve as a basis for identifying strategic technology and process initiatives over the medium to long term.

## Use this play to:

Create a holistic view of the organization and what it does, using a common language.
Serve as the starting point for aligning teams, technology architecture and domain boundaries.
Provide a stable base for identifying and prioritizing technology and process improvement initiatives.

## Expert tip

Organizations often fall into the trap of using product names or technology assets to describe what they do. To ensure you are capturing the what, use a Verb + Noun structure (e.g., Browse Catalog). This simple rule forces abstraction and gets buy-in from stakeholders on the shared language.

## Time required

1 - 2 weeks

## Who participates

Architects, business, technology, and product stakeholders

## How often

Initial mapping then review every 6 - 12 months or when strategic decisions are being made 

## Fundamentals

### Layers of a capability map

A capability map typically consists of four layers that articulate the flow of value from the market down to the enabling technology.

#### Customers
  The people or services who consume the Experience Capabilities. Can be internal or external.

  - Customer
  - Customer

  ##### Experience capabilities
  The abilities offered directly to customers (internal or external) by way of products and features.

  - Capability
  - Capability
  - ...

  ##### Business capabilities
  The core organizational functions and competencies (the what) that must be executed to deliver the Experience Capabilities. Each business capability encapsulates the processes, data, systems, events, and people that provide that capability.

  - Capability
  - Capability
  - ...

  ##### Technology capabilities
  The foundational building blocks that enable the business to build, deploy, monitor and operate applications.

  - Capability
  - Capability
  - ...

  The diagram shows a hierarchical structure where:
  - Customers consume Experience capabilities
  - Experience capabilities are delivered through Business capabilities
  - Business capabilities are enabled by Technology capabilities


### Characteristics of a capability

A capability is a building block of functionality expressed not in terms of systems or teams, but in what they enable someone to do. 
Capabilities possess intrinsic characteristics essential for architectural and organizational modeling:

* **Every capability has a customer.** This customer may be external, an internal business unit, or another capability, clarifying its purpose and value exchange.
* Capabilities are the primary blueprint for organizing modern technology teams. They **naturally lend themselves to forming independent teams** with clearly defined scope, self-contained systems, and well-defined boundaries and contracts (often exposed via APIs).
* Capabilities remain stable even as the underlying technology, processes, or organizational structure changes. They **represent long-term business value**.

### The primary focus

#### Business capabilities as the strategic anchor

While the complete capability map is a holistic visualization spanning Customers, Experience, Business, and Technology, the **Business Capability layer is the essential starting point and the true driver of organizational value.**

Enterprise Architects must initially have a sole and unwavering focus on mapping and understanding the business capabilities first. They serve as the stable anchor for your architecture because:
* **They drive strategy, not systems.**
    Business capabilities define what your organization does to deliver value, regardless of the technology used. By focusing here, you ensure your analysis is strategic and aligns directly with the business strategy.
* **They unlock value**
    Strategic decisions, such as platform boundaries, build vs. buy choices, and investment prioritization flow directly from the health and importance of your business capabilities 
* **They manage confusion**
    This deliberate focus helps mitigate two common pitfalls:
        * The technology trap: Prevent technology teams from prematurely descending into the lower technology capability layer (e.g., "our CI/CD pipeline") before the business need is understood.
        * The product/feature trap: Avoid confusion with the higher experience capability layer, which often changes with feature updates. Focusing on the enduring business function (e.g., Manage Inventory) rather than the transient customer feature (e.g., Browse Products) provides architectural stability.

Always start by mapping and assessing the business capabilities, and only then proceed to detail the experience layer above it and the technology layer that enables it.

### Domains and ownership

**Independent Domains**

To manage the complexity of technology in a large and diverse organization, boundaries must be drawn around clusters of related capabilities and technology that supports them. These clusters of capability, domains, should form natural boundaries of complexity, grouping capabilities that closely interact or evolve together.
In large enterprises, it may be useful to define subdomains within a domain to represent more specific or specialized capability areas. Subdomains provide additional clarity where variation or focus is needed without fragmenting ownership.

**Strong capability ownership**
Every capability, and by extension, each domain, requires clear business and technical ownership. A capability must be treated as a product offered to the rest of the organization. Its owner, adopting a product mindset, is accountable for ensuring the capability is valuable, usable, and continually improved to meet organizational needs.

**Why it matters**
Clear domain boundaries and ownership reduce complexity, duplication, and confusion about accountability. They enable teams to work autonomously within well-defined scopes, align technology investments to business outcomes, and support platform thinking: where capabilities are designed to be composable, reusable, and evolve over time without destabilizing the broader system.

### Definitions

Domain: A cluster of related capabilities that forms a natural complexity boundary.

Sub-domain: A smaller cluster of capability within within a domain; represents specific or specialized capability areas.

Business capabilities: Building blocks of functionality expressed not in terms of systems or teams, but in what they enable someone to do. 


### Red flags you need a capability map
Misaligned technical effort and strategic investment lead to wasted time, duplication, and slow delivery. If your organization exhibits these symptoms, a Capability Mapping play is crucial.

1. Architecture-first decision-making
Technology decisions prioritize architectural preferences (e.g., “we need 15 microservices”) over business value, customer priority, or strategic impact. Without a clear view of what the business does, architecture becomes tactical and reactive.

2. Duplicate investments
Multiple teams or business units inadvertently build the same function because they lack visibility of existing capabilities across the organization.

3. Fragmented capabilities 
A core business capability is unintentionally split across multiple teams or systems, leading to tight coupling, unclear accountability, and slower delivery.

4. Missing capabilities
Critical capabilities (especially those related to orchestration and those dormant in legacy modernization contexts) are overlooked and not captured. Missing them early can lead to costly, hard-to-reverse architectural pivots later in delivery.

5. Lack of a ubiquitous language
Teams use different terms for the same business concept. Without a shared vocabulary, identifying dependencies, duplication, and gaps is slow and manual.

6. Architectural cloning
System designs replicate legacy structures (“we had this service before, so we need it again”) instead of re-evaluating what capabilities are actually required. This preserves unnecessary complexity and blocks simplification.

## Running the play

### Capture raw input

1. Frame the work
Start by clearly defining the strategic intent and the scope of the business capability map. Are you focussed on the whole organization? Or a single business unit? Capture the business goals and vision that the business map must support. This framing prevents the map from becoming a purely academic exercise and ensures it remains strategic.

2. Identify existing resources
What already exists that you can leverage? Look for existing capability maps, business process maps, user journeys, Jobs To Be Done (JTBD), value stream maps (VSM) strategy docs, purpose, vision and goals, architecture diagrams, event storming maps, product roadmaps, and organizational charts. These artifacts contain the raw vocabulary and structure you will leverage.

3. Leverage GenAI
If your organization has access to GenAI tools, use them to accelerate your initial capability map draft.
When existing artefacts are available as described above, run them through your in-house GenAI environment to extract, cluster, and refine an initial capability view.
If you’re starting from scratch, utilise the starter prompts provided at the end of this play to generate an initial capability list for refinement.
Note: Always ensure the use of GenAI aligns with client IP and data security policies. Use only approved, internal tools. Never use un-validated GenAI output as a substitute for expert stakeholder validation.

4. Prepare the visual canvas and customers
Establish a shared, visual workspace (digital or physical). Drop the business goals and vision at the top. Then identify and list all of the customers (within the context of your framing) below the vision and goals. 
Anchors: Place any existing value streams (VSM) or JTBD loosely across the top, below the customers. This provides immediate context for the mapping. 
Layers: Create separate swimlanes for experience capabilities, business capabilities (allocate the most space here), and technology capabilities

Definitions: Clearly display the definitions for each layer and the "Verb + Noun" rule to guide participants and challenge any system (or team) based language.
Resources: Designate an area and place all raw inputs from GenAI or exiting artifacts.

5. Capture the raw mass of capabilities
Start populating your map. Focus primarily on business capabilities, but capture experience and technology capabilities as they emerge. The goal is velocity over perfection; get a mass of capabilities on the canvas. Loosely align them to the VSM/JTBD anchors (or customers/goals if VSM/JTBD are absent). Do not worry about domains or hierarchy yet.

#### Refine and align

6. Clean, cluster, and validate language
Group the raw capabilities into related clusters. Refine terminology into the Verb + Noun structure, abstracting away product names. As you clean, move Experience and Technology items to their appropriate layers. Capture duplicates as they are, do not merge them yet; this highlights intentional or accidental duplication.

7. Define and name domains
Take the capability clusters and define Domain names for each. These must be your future state groupings, focused on creating a natural complexity boundary around functions. Note: These domains will likely contradict current organizational team alignments, and that is okay.

8. Validate and seek feedback
Share this early draft with stakeholders in short, focused 1:1 or small group sessions (e.g., 60 minutes).
Ask: What's missing?; Why do these duplicates exist?; Have we accurately captured what you do?
Let them correct your errors; capture all feedback, language suggestions, and additional context without debate. Your work is to facilitate their insight.

### Finalization and adoption

9. Final language and consistency check
Work in the feedback from validation sessions. Review all capabilities to ensure adherence to the Verb + Noun rule (no product or system names). 
Ensure visual consistency (even spacing, block sizes, colors). Add supporting context, such as short definitions for each domain and capability if needed. 

10. Confirm alignment
Share the final map back with key stakeholders. Clearly state that the domains represent a future state view. Use colors to highlight any identified duplicate capabilities and the new capabilities (gaps) identified in the process.

11. Publish and socialize
Publish the map in a highly accessible, living location (e.g., Confluence, Mural). Run an "Architectural Show-and-Tell" session to walk people through the map, highlight the strategic takeaways, and encourage its use in all future investment and design discussions.

## Tips

### Capability mapping tips

* Keep it simple
Don't worry about multi-level hierarchies (Level 1, 2, 3 capabilities); often, a clear two-level grouping (Domain -> Capability) is sufficient and less complicated.
* Keep it visual
A clear, well-spaced visual map creates shared understanding and invites meaningful engagement from across the organization.
* Organize for flow 
When defining domains, aim to organize them based on the flow of value (e.g., Customer Journey), as this naturally aligns with the principles of Domain-Driven Design and Team Topologies.
* Prioritize buy-in over pedantry
The success of the map relies on stakeholder adoption, not linguistic perfection. If a stakeholder insists on specific terminology, document and proceed. Do not engage in lengthy debates over naming conventions, as this derails momentum and jeopardizes buy-in. Your ubiquitous language will evolve naturally; trust that clearer terminology will surface organically through continued use and iteration.
* Recognize organizational bias
Feedback from stakeholders can often be driven by attachment to existing implementations (teams, systems, products) rather than the stable, objective capability. Note that fear of change or loss of team ownership can color advice. Your role is to strategically filter the emotional bias from the domain expertise.
* Check against team topologies
Ensure your proposed domains support the creation of streamline-aligned teams and clarify which capabilities belong to enabling, platform, or complicated sub-system teams.

