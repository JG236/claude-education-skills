# Domain 14: Skill Specifications — For Review Before Building
*Draft for Gareth Manning's approval. Claude Code builds nothing until this is approved.*
*Four skills in this draft: SEEDS, Band System, LT Authoring, Rubric Logic.*
*D2R and Habit Design Curriculum added later after separate briefing sessions.*

---

## Framing Language for All Domain 14 Skills

Every skill in this domain opens its "What This Skill Does" section with:

> *"This skill encodes an original practitioner framework developed by Gareth Manning, educator, curriculum designer, and learning systems designer. Unlike skills in other domains, it is not drawn from peer-reviewed research traditions. It is grounded in serious engagement with learning science, original curriculum design work, and active classroom testing. It is included because the methodology is coherent, transferable, and genuinely useful — and because intellectual honesty requires distinguishing practitioner frameworks from research-validated approaches."*

---

## Skill 1: SEEDS Regenerative Inquiry Cycle

**skill_id:** `original-frameworks/seeds-regenerative-inquiry-cycle`
**evidence_strength:** `emerging` (practitioner framework, not peer-reviewed)

**What it does:**
Designs a SEEDS inquiry cycle for early childhood and primary contexts — a five-stage regenerative learning process that grounds student inquiry in real places, real systems, and real care. SEEDS stands for **Sense → Envision → Experiment → Design to Last → Share**. Unlike linear project frameworks, SEEDS is cyclical — Share connects back to Sense, and each stage overlaps and recurses. Unlike most project-based learning frameworks, SEEDS begins with attunement and bio-empathy rather than a problem statement, and ends with stewardship structures rather than a presentation. The output is a full SEEDS cycle plan including stage-by-stage guidance, documentation approach, and stewardship design.

**Evidence foundation to encode:**
- Manning's SEEDS cycle (2025) — the framework itself, published in *All Thoughts Subject to Change* (Substack)
- Inspired by but distinct from Green School Bali's 4S model (Freud) — acknowledges the catalyst while being clear SEEDS is original development with significantly different assessment philosophy
- Philosophical underpinning: Vervaeke's relevance realisation (Sense stage), Kimmerer's *Braiding Sweetgrass* on bio-empathy and reciprocity, Sterling's sustainable education
- Reggio Emilia documentation pedagogy (aligned with but independent of SEEDS assessment approach)
- Place-based education evidence (Sobel, Castagno & Brayboy) as external validation of the underlying principles
- Regenerative vs restorative vs sustainable spectrum (from Metabolising Regeneration, Manning 2025)
- Robin Wall Kimmerer quote as philosophical anchor: *"This is our work. To discover what we can give."*

**Input schema (required):**
- `learning_group`: Which age group (early childhood 5–8 / primary 8–12)
- `place_context`: The specific place, ecosystem, or community that anchors the inquiry

**Input schema (optional):**
- `existing_problem_or_potential`: A known issue or opportunity, if identified — SEEDS may begin from problem or from possibility
- `time_available`: Term length, year-long, or shorter cycle
- `community_connections`: People, organisations, or ecosystems available
- `documentation_approach`: How learning will be made visible (learning stories, portfolios, observations)

**Output schema:**
- `seeds_overview`: Summary of the cycle, place anchor, and regenerative intent
- `sense_stage`: Attunement activities, bio-empathy practices, baseline data gathering, knowledge gap identification
- `envision_stage`: Ideation sequence, expert engagement plan, criteria-based reality testing, assessment checkpoints
- `experiment_stage`: Prototyping and action plan, adaptation mechanisms, formative assessment approach
- `design_to_last_stage`: Stewardship structure, care routines, handoff plan, named steward or successor
- `share_stage`: Impact assessment (honest — positive, negative, intended, unintended), storytelling approach, connection back to Sense
- `documentation_plan`: How learning is made visible throughout — portfolios, learning stories, observations
- `known_limitations`: Honest framing about evidence base, time requirements, tension with standard school timelines

**Chains well with:** place-based-inquiry-anchor, reggio-documentation-protocol, ecological-inquiry-anchor-designer, ubuntu-collective-knowledge-task-designer

**Key distinctions to encode in the prompt:**
- SEEDS is cyclical, not linear — Share feeds back into Sense
- Begins with quality of attention, not identification of a problem
- Bio-empathy includes non-human voices — not just human stakeholder empathy
- Assessment is documentation-based throughout, not product-focused at the end
- "Design to Last" is not the same as "present" — stewardship is the point
- The regenerative spectrum matters: restorative is minimum, regenerative is the aim
- It is better to stay in Envision and become knowledgeable than to act unknowingly and cause harm

---

## Skill 2: Developmental Band System Designer

**skill_id:** `original-frameworks/developmental-band-system-designer`
**evidence_strength:** `emerging` (practitioner framework grounded in developmental psychology)

**What it does:**
Designs a developmental band system for a competency-based curriculum — a framework that specifies what competent looks like at each broad developmental stage rather than each individual grade level. Solves a problem that most competency frameworks ignore: the difference between what competent means for a 6-year-old versus a 12-year-old. The output is a complete band architecture for a school or programme, including the number of bands, their developmental rationale, age/grade mapping, and the logic for the exceptions (subjects requiring finer granularity).

**Evidence foundation to encode:**
- Manning's developmental band system (original — active since REAL School Budapest implementation)
- Critique of flat competency lists: UNESCO AI competency frameworks, most national curriculum frameworks — list competencies without developmental specificity, leaving teachers to infer what competent means at each age
- Piaget's stages of cognitive development as developmental anchor — concrete operational (Band B, ages 8–10), formal operational (Bands C–D, ages 10–14) — used as rationale, not as rigid prescription
- Mixed-age grouping research (Montessori, Vygotsky ZPD) — bands support rather than undermine mixed-age learning by specifying competence at the band level rather than grade level
- Wiggins & McTighe backwards design as the starting point — but extended to include the "why" layer Manning adds before UBD's "what" layer
- Manning's critique of UBD: teachers in standard UBD are never asked why — they're given curriculum goals and work backwards from there. Purpose-driven backwards design starts earlier: mission → values → competency priorities → LT decomposition → band specification

**Input schema (required):**
- `school_mission`: The core purpose and values of the school or programme
- `age_range`: The full age range the band system needs to cover
- `programme_context`: What kind of learning (PBL, subject-based, hybrid)

**Input schema (optional):**
- `existing_competency_framework`: Any existing framework being mapped (EU frameworks, UNESCO, national curriculum)
- `mixed_age_groupings`: Whether the school uses mixed-age learning groups
- `subject_exceptions`: Subjects that require finer granularity than broad bands (maths, language acquisition)

**Output schema:**
- `band_architecture`: Number of bands, age/grade mapping, developmental rationale for each band break
- `developmental_rationale`: Why the bands are where they are — cognitive and social-emotional development reasoning
- `competent_definition_logic`: How to determine what competent means at each band (not a list of topics but a developmental description of capability)
- `exception_handling`: Which subjects need finer granularity and why, with guidance on 9-level or similar precision systems
- `mixed_age_implications`: How the band system supports rather than undermines mixed-age learning
- `known_limitations`: Bands are broad — some students will be significantly ahead of or behind their band. How to handle this honestly.

**Key distinctions to encode in the prompt:**
- The goal is developmental precision without manageability cost — not so granular that teachers can't plan to it, not so broad that it's meaningless
- Bands map to multi-year groups deliberately — a student can be in Band B for two years, assessed against the same Competent line, growing within it
- The critique of flat competency lists is central — encode why this problem matters and what it costs teachers and students when it isn't solved
- Purpose-driven backwards design sequence: mission → values → what the curriculum must prioritise → what it must not prioritise → competency selection → LT decomposition → band specification
- "Spiky learners" over "well-rounded students" — the band system supports depth and strength, not uniformity

---

## Skill 3: Purpose-Driven Learning Target Authoring Guide

**skill_id:** `original-frameworks/learning-target-authoring-guide`
**evidence_strength:** `emerging` (practitioner framework with strong grounding in assessment research)

**What it does:**
Guides an educator or curriculum designer through writing a complete, coherent set of learning targets (LTs) for a competency — from the upstream question of whether the competency is right, through decomposition into 2–3 LTs, to writing band-level statements that are developmental, precise, and assessable. The output is a complete LT set ready for use in planning and reporting, with quality checks built into the process.

**Evidence foundation to encode:**
- Manning's LT authoring methodology (original — developed and refined at REAL School Budapest, documented in Learning Target Authoring Guide v3.1, January 2026)
- Formative assessment research (Black & Wiliam 1998) — clear learning intentions are prerequisite for effective formative assessment
- Wiggins & McTighe backwards design — extended with Manning's upstream "why" layer
- Observable and measurable learning objectives (Bloom's taxonomy verbs) — the prohibition on "understand/know/appreciate" and the preference for identify/describe/compare/explain/justify/analyse/evaluate/create
- Developmental progression levers: independence, complexity, scope, precision, reasoning, transfer — these are the mechanisms of progression, not topic escalation
- Vygotsky's ZPD — band statements specify the upper edge of what students can do with appropriate support at that developmental stage

**Input schema (required):**
- `competency_name`: The broad capability being decomposed
- `competency_definition`: One sentence beginning "The ability to..."
- `band_range`: Which bands this LT set covers
- `programme_purpose`: Why this competency matters for this school's mission

**Input schema (optional):**
- `existing_draft`: Any existing LT wording to review and revise
- `subject_area`: The curriculum domain
- `assessment_context`: How LTs will be used — reporting, project assessment, or both

**Output schema:**
- `competency_review`: Is this competency right? Does it serve the mission? Is it genuinely a capability or a topic list in disguise?
- `lt_decomposition`: The 2–3 LTs that make the competency actionable, with rationale for each
- `lt_definitions`: One-sentence "I can..." definitions for each LT
- `band_statements`: Full A–D progression for each LT using the appropriate progression levers
- `quality_check`: Running through the checklist — single-construct rule, no inline examples, observable verbs, vertical coherence, horizontal coherence
- `known_limitations`: Where the LT set is strongest; where teacher judgment will still be needed

**Key rules to encode in the prompt (from the authoring guide):**
- Every band statement begins "I can..." — present tense, active voice
- No parentheses, no inline examples, no "such as" or "for example" anywhere
- Single-construct rule — one coherent capability per statement, "could I assess these separately?" test
- Prefer observable action verbs: identify, describe, compare, explain, justify, analyse, evaluate, create
- Avoid: understand, know, appreciate, sophisticated, effectively, well (without observable criteria)
- Progression uses levers (independence, complexity, scope, precision, reasoning, transfer) — not topic escalation
- 2 LTs per competency is the default; 3 only if strands are genuinely distinct
- The LT definition must describe what ALL band levels do — it's the generalised statement, not Band A

---

## Skill 4: Coherent Rubric Logic Builder

**skill_id:** `original-frameworks/coherent-rubric-logic-builder`
**evidence_strength:** `emerging` (practitioner framework grounded in assessment and learning science)

**What it does:**
Builds a complete, coherent rubric for a learning target or project assessment — using a five-level scale where Competent IS success, not a midpoint. The output is a full rubric table with precise descriptors at each level, plus a co-construction plan for working with students to make the criteria their own. Designed to be used alongside the LT authoring guide — the rubric is the assessment instrument for a specific LT or product, not a separate system.

**Evidence foundation to encode:**
- Manning's rubric logic (original — documented in REAL School Rubric Logic Guide v2.1, January 2026)
- Competency-Based Education philosophy — Burch's four stages of competence (unconscious incompetence → conscious incompetence → conscious competence → unconscious competence) as the developmental model underlying the five levels
- Haring et al. (1978) Instructional Hierarchy — acquisition, fluency, retention, generalisation, adaptation — maps to rubric levels and determines appropriate homework and independent practice
- Black & Wiliam (1998) formative assessment — rubrics are only useful if they change teaching and learning decisions; the co-construction process is essential for this
- Sadler (1989) on standards and quality judgement — students need to understand what quality looks like before they can self-assess meaningfully
- Exemplar analysis as the foundation of co-construction — students analyse strong, average, and weak examples before generating criteria language

**Input schema (required):**
- `learning_target`: The exact LT band statement being assessed
- `band`: Which developmental band this rubric is for
- `product_or_performance`: What students will produce or do to demonstrate the LT

**Input schema (optional):**
- `student_level`: Age/year group for language calibration
- `formative_or_summative`: Whether this is a checkpoint rubric or a final assessment rubric
- `compound_lt`: Whether the LT contains distinct sub-skills that warrant splitting

**Output schema:**
- `teacher_rubric`: Full five-level table (No Evidence / Emerging / Developing / Competent / Extending) with precise descriptors — work-facing language, word limits respected, distinct levels with no overlap
- `co_construction_plan`: How to work with students to generate student-friendly criteria language through exemplar analysis
- `student_rubric_template`: The student-facing version with accessible language (Not yet / Getting there / Got it! / Wow!)
- `written_feedback_guide`: How to write specific, actionable feedback for each level
- `known_limitations`: Where professional judgment is still needed; what the rubric can't do

**Key logic to encode in the prompt:**
- Five levels: No Evidence / Emerging / Developing / Competent / Extending
- **Competent IS success** — it is not average, not "good enough" — it represents genuine mastery of the band-level expectation. This is the single most important design principle.
- Extending is rare — it requires specific evidence of transfer, depth, sophistication, or teaching others. It is not a motivational tool.
- Emerging is a legitimate starting point — it is not failure. All learners begin here.
- Developing is not a punishment — it is a natural and expected stage of growth on the way to Competent
- Quantitative equivalents (0% / 1–49% / 50–74% / 75–89% / 90–100%) are calibration guides, not targets
- Word limits: No Evidence ≤10 words / Emerging ≤15 / Developing ≤20 / Competent ≤25 / Extending ≤20
- Work-facing voice throughout — describe the work, not the student ("Shows clear structure" not "You showed clear structure")
- Compound LTs: split only when pedagogically justified; summative judgment rule (Competent on majority, none below Developing)
- Co-construction sequence: teacher prepares rubric → students analyse exemplars → students generate criteria language → teacher maps to formal criteria → both versions published
- Connection to instructional hierarchy: a student at Emerging needs guided practice, not more homework; a student at Competent is ready for independent application

---

## What's Not Here Yet

**D2R 7-Stage Process** — Gareth to confirm with Barna whether the school is happy for this to be shared publicly. If yes, builds as a separate skill with full stage documentation.

**Habit Design Curriculum Sequence** — Gareth to confirm when the Strive curriculum logic is stable enough to encode. Placeholder held in Domain 14.

**Competency Framework to Developmental Band Mapper** — builds naturally after the above two are confirmed. Requires knowing the D2R competency structure to encode the mapping logic properly.

---

*Review this document carefully. If the framing, evidence foundation, key distinctions, or input/output schemas for any skill are wrong or incomplete, say so before Claude Code builds anything. Once you approve, I'll write the Claude Code prompt.*

---

## Skill 5: Self-Determined Project Design Protocol

**skill_id:** `original-frameworks/self-determined-project-design-protocol`
**evidence_strength:** `emerging` (practitioner framework grounded in SRL and deliberate practice research)

**What it does:**
Guides both student and educator through the full arc of designing, planning, and executing a self-determined personal project — from initial idea through to completion, defence, and reflection. Specifies what both parties need to do at each phase, how to calibrate ambition honestly, and how to build the knowledge and skill acquisition plan alongside the project itself. Output is a complete dual-perspective protocol: student-facing roadmap and educator-facing mentoring guide, phase by phase.

**Evidence foundation:**
- Manning's personal project mentoring methodology (original — developed through LD capstone mentoring and prior international teaching)
- Zimmerman (2000, 2002) self-regulated learning — forethought, performance, self-reflection phases map directly to the protocol sequence
- Bandura (1997) self-efficacy — feasibility calibration is fundamentally about honest self-efficacy assessment; over-ambitious and under-ambitious projects both reflect miscalibrated self-efficacy
- Ericsson & Pool (2016) deliberate practice — the knowledge/skill acquisition plan is a deliberate practice design problem
- Wiggins & McTighe backwards design — extended with Manning's upstream "why" layer
- Black & Wiliam (1998) formative assessment — milestone checkpoints function as structured formative assessment moments
- Manning's rubric logic and LT authoring methodology (Domain 14 Skills 3 and 4) — embedded in Phase 3

**Input schema (required):**
- `student_idea`: The student's initial project idea — however rough
- `student_level`: Developmental band and age
- `available_time`: Total duration and weekly time commitment

**Input schema (optional):**
- `existing_curriculum_LTs`: Whether curriculum LTs exist for this domain or need to be created
- `mentor_expertise`: How much the educator knows about the project domain
- `prior_experience`: What the student has already done in this area

**Output schema:**
- `phase_1_ideation_and_feasibility`: Student actions + educator actions — idea articulation, feasibility reality-check, possibility expansion if needed
- `phase_2_knowledge_gap_analysis`: Parallel research by student AND educator — what's required, what the student knows, what they don't, honest readiness assessment
- `phase_3_planning`: LT selection or creation, exemplar analysis, rubric development, knowledge/skill acquisition plan, timeline with milestones, resource and mentor identification, tracking system setup
- `phase_4_execution_and_monitoring`: Weekly rhythm, self-monitoring protocol, milestone check-ins, adaptive replanning
- `phase_5_completion_and_defence`: Final self-assessment against rubric, presentation or defence, honest impact assessment
- `tracking_system`: Specification for the shared visible artefact — doc, board, or sheet — that both student and mentor can see at all times. Must show: the plan, the timeline, current status against milestones, and evidence of progress. Tool-agnostic (Trello, Google Doc, sheet, or dedicated app) but functional requirements are non-negotiable. This is also the specification an AI tool would build to.
- `educator_feasibility_calibration_guide`: Specific questions to determine genuine readiness — what students should be able to explain, what to do when they're not ready
- `known_limitations`: Where the protocol requires the educator to reach outside their expertise; when to bring in external mentors

**The five phases — encode this sequence precisely:**

Phase 1: Student arrives with idea. Educator listens without deflating. What do you want to make? Who is it for? Why does it matter? What would success look like? Then honest feasibility conversation — probing ambition calibration without crushing agency.

Phase 2: Parallel research. Student researches what knowledge and skills the project requires. Educator does the same independently. They meet, compare findings, have honest conversation. If student can't explain core concepts when asked directly, that's the data. Educator brings in external expert if domain is outside their knowledge.

Phase 3: Planning — only after feasibility established. Select or create LTs. Analyse exemplars. Co-construct success criteria and rubric. Design knowledge/skill acquisition plan. Build timeline with milestone checkpoints. Identify mentors or experts. Set up shared tracking system.

Phase 4: Execution with structured monitoring. Weekly self-monitoring using tracking system. Milestone checkpoints: self-assess against rubric, share evidence, get feedback, adapt plan. Timeline is a living document. Break into smaller chunks when needed.

Phase 5: Final self-assessment against rubric. Presentation or defence. Honest reflection on what was achieved, what wasn't, what was learned about the process.

**Key distinctions:**
- Educator researches independently before feasibility meeting — feedback is authoritative, not just encouraging
- Knowledge/skill acquisition plan runs in parallel with project plan — you learn what you need as you build
- LTs and rubric before execution — students who understand excellence produce better work
- Tracking system is shared and visible to both parties at all times — not a private student document
- Over-ambitious equals under-ambitious in terms of harm — a student who fails a project they weren't ready for learns the wrong lesson
