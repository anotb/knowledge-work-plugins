# Master Outstanding Items (Updated Post-R4)

## Structural Changes
- [x] Merge: report-generation + executive-presentation → "client-deliverables" (DONE)
- [x] Merge: problem-solving + strategic-frameworks → "strategic-analysis" (DONE)
- [x] Update README for 15 skills (DONE)
- [x] Clean up empty directories after merges (DONE)
- [x] Create CLAUDE.md with writing style (DONE, no skill count hardcoded)
- [ ] README: Update to Cowork-first convention (opening line, installation sections, settings)
- [ ] README: Remove "Agent Skills open standard" / "20+ agents" language (doesn't match repo convention)
- [ ] Update plugin.json if needed

## R4 Feedback: What Would Get Each Skill to Perfect

### Cross-Cutting (applies to most skills)
- [ ] AI tells (7-8/10): Outputs are too uniformly polished. Real consulting has rougher edges, crossed-out sections, "TBD" notes. Consider adding guidance like "prioritize depth on the 2-3 most critical sections rather than even coverage across all"
- [ ] Contextual reasoning boundary: Risk probability scores, timeline estimates are "informed estimates" not backed by data. Consider flagging these more explicitly
- [ ] Some skills produce "frameworks ready for population" rather than "findings" when given limited data. This is CORRECT behavior but could acknowledge the limitation more naturally

### problem-solving (pride 9, avg 8.6)
- [ ] R4 noted it's close to perfect. Minor: could be slightly less structured in initial response (real consultants start messier)

### strategic-frameworks (pride 9, avg 8.8)
- [ ] Market sizing section sometimes omitted when it would be relevant
- [ ] Could push harder on "what's the non-obvious connection" across frameworks

### financial-modeling (pride 9, avg 8.8)
- [ ] The self-correction behavior ("wait, this doesn't work") is excellent but could be more natural/less formulaic
- [ ] DCF section still thinner than the business case section

### executive-presentation (pride 8, avg 8.0)
- [ ] Could push harder on PE-specific angles (fund return hurdles, exit timeline)
- [ ] Backup slide descriptions too neat (real appendix lists are messier)

### report-generation (pride 8, avg 8.2)
- [ ] Insight is in structure/logic, not novel findings (inherent limitation but could coach for more "so what")
- [ ] Could benefit from deliberate imperfection: "We were unable to confirm X"

### change-management (pride 8, avg 8.4)
- [ ] Plan length could be trimmed for specific audiences
- [ ] Cultural archetype guidance is good but could be tested with more diverse scenarios

### due-diligence (pride 8, avg 8.2)
- [ ] Strong on refusing to fabricate. Could push harder on asking for specific data items interactively
- [ ] Working capital analysis for capital-intensive services still not deeply covered

### engagement-pricing (pride 7, avg 7.6)
- [ ] Gap between "help me price this" and "here's a framework for pricing it" is real
- [ ] Could push harder to get rate card interactively BEFORE building framework
- [ ] Still the weakest-scoring skill - needs focused attention

### thought-leadership (pride 8, avg 8.2)
- [ ] Slight TED-talk sheen remains in places ("the gap is widening")
- [ ] Could use more rougher edges, surprising findings, acknowledged limitations
- [ ] Voice is good but could be sharper/more contrarian

### engagement-setup (pride 8 est., waiting on R4-Eval-3)
- [ ] Comprehensive but could be tighter for a real internal document

### proposal-development (pride 7 est., waiting on R4-Eval-3)
- [ ] Government/public sector proposals need firm-specific content (past performance, team names)
- [ ] Framework vs populated output tension

### implementation-planning (pride 8 est., waiting on R4-Eval-3)
- [ ] Could strengthen the "So What" moment between analysis and recommendation

### org-design (pride 8, avg 8.2)
- [ ] Could be tested with more ambiguous prompts to expose weaknesses
- [ ] Matrix management guidance is good but specific examples could be richer

### process-excellence (pride 8, avg 8.4)
- [ ] Solution evaluation matrix correctly leaves impact blank - but user needs guidance on next iteration
- [ ] Industry benchmarks section could be expanded beyond O2C, P2P, R2R

### project-governance (pride 8, avg 8.2)
- [ ] Stage gate timing stated with confidence that should be flagged as indicative
- [ ] Could benefit from executive summary page at top

### project-closeout (pride 8, avg 8.4)
- [ ] Phase 2 handling is strong. Internal coaching vs client-facing content could be separated
- [ ] Closeout effort estimation could be more precise

### workshop-facilitation (pride 9, avg 8.6)
- [ ] Strongest skill in the library. Minor: contingency plan for when day runs long
- [ ] Pre-brief scripts are the most valuable element - could be even more specific

## Quality Gates Before PR Submission
- [ ] Second AI slop pass on merged skills
- [ ] Frontmatter validation on merged skills
- [ ] Description optimization for merged skills (new trigger terms needed)
- [ ] Verify no regressions from merges (eval merged skills)

## Track 3: Standalone Repo
- [ ] Sync ALL improvements to standalone repo
- [ ] Update standalone README for 15 skills
- [ ] Commit and push

## Track 4: PR Submission (3 PRs)
- [ ] Remove EVAL_IMPROVEMENTS.md and OUTSTANDING.md from submission
- [ ] Comment on PR #51 (brief, linking to new PRs)
- [ ] PR 1: Core analytical skills (scaffolding + ~6 skills)
- [ ] PR 2: Engagement lifecycle skills (~5 skills)
- [ ] PR 3: Strategy & transformation skills (~4 skills)
- [ ] Cross-link all PRs

## Track 5: Other PRs
- [ ] Update PR #384 on anthropics/skills
- [ ] Refresh awesome-claude-skills PRs (5 open)
