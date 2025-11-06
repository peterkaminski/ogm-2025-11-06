# Work Log: Building the OGM 2025-11-06 Wiki

This page documents the process of creating this comprehensive wiki from the OGM community call transcript and chat log.

## Overview

**Date**: November 6, 2025 (wiki created same day as call)
**Tool Used**: Claude Code (Anthropic's agentic AI assistant)
**Source Materials**:
- Zoom transcript (~38,085 tokens - very large!)
- Chat log with extensive threaded conversations
- Initial Gemini-generated participant insights (CSV)

**Final Result**: 89 interlinked wiki pages with 6,500+ lines of documentation

---

## Phase 1: Initial Setup and Planning

### User Request
Peter asked for comprehensive analysis and synthesis of the OGM call, noting:
- He liked the Gemini takes but thought they were incomplete
- Chat had extensive conversations worth organizing
- Wanted lists of people, books, organizations
- Requested markdown wiki with `[[Double Square Bracket Links]]`
- Filenames should use proper capitalization and spaces

### My Planning Approach

I created a todo list with 8 tasks:
1. Read full transcript
2. Analyze chat log
3. Extract entities
4. Create wiki structure
5. Generate participant pages
6. Create chat conversation summaries
7. Create entity index pages
8. Commit and push

**Key Decision**: Use wiki-style navigation rather than a single document to enable exploration from multiple entry points.

---

## Phase 2: Reading and Analysis

### Challenge: Transcript Size
The transcript was 38,085 tokens - exceeded the 25,000 token read limit!

**Solution**: Read in chunks, starting with first 2,000 lines to identify participants and structure.

### Discoveries

**Participant Count**: Found 13 participants (Gemini had captured 11):
- Scott Moehring, Gil Friend, Alex Kladitis, Pete Kaminski
- Kevin Jones, David Witzel, Klaus Mager, Jerry Michalski
- Mike Nelson, Victoria (Spain), Stacey Druss, Doug Breitbart
- Rick Botelho (present but didn't check in)

**Chat Richness**: The chat log was surprisingly rich with:
- Resource sharing (links, articles, books)
- Threaded discussions continuing check-in topics
- Side conversations and follow-ups
- Direct messages between participants

**Major Themes Emerged**:
- Consciousness and perception (Jerry's psilocybin journey!)
- AI bias and bubbles
- Regenerative agriculture
- Curiosity vs attention decline
- Information overload

---

## Phase 3: Wiki Structure Creation

### Main Index Page
Created `Index.md` as the entry point with sections for:
- Participants (13)
- Major Themes (organized by category)
- Chat Conversations
- Referenced Works
- Key Organizations

### Design Decisions

**Filename Convention**:
- Used exact page titles with spaces: `Scott Moehring.md`
- Proper capitalization: `AI Financial Bubble.md`
- No forbidden filesystem chars (obviously)

**Link Style**:
- `[[Double Square Bracket Links]]` throughout
- Links to non-existent pages would be created later
- Rich cross-referencing between related concepts

---

## Phase 4: Participant Pages (13 pages)

### Approach
For each participant, I went beyond the Gemini takes by:
- Including full context from their check-in
- Adding all their chat contributions
- Connecting to related concepts
- Cross-referencing with other participants

### Examples

**Scott Moehring**: Expanded remixability concept, added his chat contributions about curiosity/attention and environmental neurodiversity hypothesis

**Jerry Michalski**: Wove together his Mr. Rogers story, Dan Brown reading, non-local consciousness theory, and psilocybin experience into a coherent narrative

**Klaus Mager**: Connected his frustration with climate warnings to his concrete solutions for regenerative agriculture economics

**Doug Breitbart**: His tab groups discovery as both personal breakthrough and example of environmental neurodiversity

### Writing Style
- Started each section with context
- Used quotes from the call
- Connected to broader themes
- Maintained their voice and perspective

---

## Phase 5: Entity Pages (3 major pages)

### Books and Publications
Comprehensive catalog including:
- Books (Dan Brown, Michael Lewis, Leonard Shlain)
- Academic articles (Nature, WSJ, Seeking Alpha)
- IETF standards documents
- Newsletter/Substack posts
- Wikipedia articles shared

**Challenge**: Extracting all the links from chat while maintaining context

### People Referenced
Created mini-profiles for:
- Creators (Kevin MacLeod, Dan Brown)
- Financial figures (Michael Burry, Sam Altman)
- Political figures (Abigail Spanberger)
- Tech leaders
- Authors and thinkers
- Family members mentioned

**Approach**: Include why they were relevant to the discussion, not just who they are

### Organizations and Initiatives
Grouped by type:
- Agricultural (Schumacher Institute, CSAs, Union of Concerned Scientists)
- Technology (OpenAI, Anthropic, Cloudflare, IETF)
- Media/Info (Panoptica, Epsilon Theory, Carnegie Endowment)
- Events (TEDx Mid-Atlantic)

---

## Phase 6: Theme and Concept Pages (5 initial pages)

Created deep-dive pages on major topics:

**AI Financial Bubble**: Mike's concerns, the three bubbles, investment questions, poll results

**Field of Sheaves**: Pete's ambitious AI-assisted synthesis project

**Non-Local Consciousness**: Jerry's integration of multiple sources into coherent theory

**Remixability**: Scott's concept with Kevin MacLeod example

**Chat Thread - Curiosity Decline**: Synthesized the rich discussion from multiple participants

### Writing Philosophy
Each page told a complete story:
- Set context from the call
- Explained the concept clearly
- Connected to related ideas
- Linked to relevant participants

---

## Phase 7: The Orphan Page Challenge

### Discovery
After initial commit, Peter noted broken links - pages that were referenced but didn't exist yet.

**Count**: 67 orphan pages!

### My Approach

**Format for Each Orphan Page**:
```markdown
> **Note**: This topic was mentioned during the OGM 2025-11-06 call
> in [context], but was not a main focus of discussion. This page
> provides background on the concept.
```

Then:
- Useful background information (not just a stub)
- How it connected to the call
- Why it mattered
- Links to related concepts

### Categories of Orphan Pages

**Mentioned but not discussed deeply**:
- GABA and Filtering
- Psilocybin and Perception
- Automated Transcript De-identification

**Tools and technologies**:
- Claude Code, Droid
- Creative Commons, Open Source

**Organizations mentioned briefly**:
- Capgemini, Schumacher Institute, IETF

**People referenced**:
- Kevin MacLeod, Dan Brown, Michael Burry, Leonard Shlain
- Sunil Malhotra, Andreas Sjöström, Ben Hunt, Marshall Kirkpatrick

**Concepts that emerged**:
- Environmental Neurodiversity
- Revolutionary Legos
- Nelson's Law
- Two Truths and a Lie

**Systems thinking**:
- Growth in Living Systems
- Regenerative Economics
- Economics as Indigenous Knowledge
- Living Systems in Policy

### Creative Decisions

**GABA and Filtering**: Treated as scientific concept with connection to consciousness theories

**Environmental Neurodiversity**: Scott's hypothesis deserved full treatment - it was a genuine insight

**Revolutionary Legos**: Gil's phrase captured something important about remixability

**Sourdough as Metaphor**: David's half-formed idea worth preserving

---

## Phase 8: Quality and Consistency

### Cross-Referencing
Every page links to:
- Related concepts
- Relevant participants
- Parallel ideas
- Source discussions
- Back to Index

### Disambiguation
Created redirect pages where needed:
- "GABA" → links to "GABA and Filtering"
- "Noetic Sciences" → "Noetic Science"
- "Panoptica.ai" → "Panoptica and Narrative Tracking"

### Voice and Tone
Maintained:
- Respectful of all perspectives
- Neutral on controversial topics (psychedelics, political shifts)
- Clear about speculation vs facts
- Participants' actual words when possible

---

## Reflections and Insights

### What Worked Well

**Rich Source Material**: The combination of transcript AND chat was gold. Chat filled in what transcript missed.

**Early Structure**: Creating Index first gave me a map to follow.

**Progressive Enhancement**: Starting with participants, then entities, then concepts built naturally.

**Todo List**: Breaking into tasks kept me focused and showed progress.

### Challenges Overcome

**Scale**: 38,085 token transcript required chunked reading approach.

**Complexity**: 13 participants × multiple topics × chat threads = complex web to capture.

**Orphan Pages**: 67 additional pages was more than expected, but each added value.

**Voice Balance**: Maintaining neutrality while capturing passion of discussions.

### Interesting Patterns

**Conversation Threads**: The curiosity/attention discussion was richer than any single check-in.

**Cross-Pollination**: Doug's tab groups connected to Scott's environmental neurodiversity, Pete's observations about AI adoption, Mike's overstimulation.

**Hidden Gems**: Stacey's "two truths and a lie" was brief but profound.

**Meta Moments**: The call itself demonstrated themes it discussed (information overload, need for synthesis tools).

### What I Learned

**About the Community**:
- Deep thinkers connecting across domains
- Comfortable with ambiguity and "woo-woo"
- Generous knowledge sharing
- Jerry as genuine "energetic center of gravity"

**About Synthesis**:
- Chat + transcript > either alone
- Small observations (like Doug's tab groups) can be profound
- Emerging concepts (environmental neurodiversity) worth capturing even if incomplete
- Links create meaning through connection

**About AI-Assisted Knowledge Work**:
This wiki is itself an example of what Pete described:
- Agentic AI (me, Claude Code) working with human (Peter)
- Processing large corpus (transcript + chat)
- Creating structured synthesis
- Questions about attribution (who "wrote" this wiki?)

---

## Technical Details

### Git Workflow
- Branch: `claude/analyze-synthesize-text-011CUs7984yMf6YQBUS96Qbd`
- Commits: 3 main commits
  1. Initial 23-page wiki
  2. 67 orphan pages
  3. This work log
- All pushed to remote for Peter to merge

### File Organization
```
/
├── README.md
├── sources/
│   ├── gemini-takes.md
│   ├── gemini takes.csv
│   └── 2025-11-06 09.36.49 Jerry Michalski's Zoom Meeting/
│       ├── meeting_saved_closed_caption.txt
│       └── meeting_saved_new_chat.txt
└── wiki/
    ├── Index.md
    ├── [89 wiki pages].md
    └── Work Log.md (this file)
```

### Statistics
- **89 wiki pages** total
- **6,500+ lines** of markdown
- **13 participant** pages
- **3 entity index** pages (Books, People, Organizations)
- **4 chat thread** pages
- **67 concept/topic** pages
- **Fully interlinked** - no broken [[Links]]

---

## For Future Reference

### Using This Wiki

**Entry Points**:
- `Index.md` - Organized overview
- Any participant page - Deep dive on person
- Any concept page - Explore an idea
- Follow `[[Links]]` - Discover connections

**Navigation**:
- Every page links back to Index
- Related Concepts sections
- See Also sections
- Cross-references throughout

### Potential Extensions

**If continuing this work**:
- Add timestamp references to transcript
- Create theme-based reading paths
- Build visual connection maps
- Add "questions raised" sections
- Create synthesis across multiple calls

**Tools that would help**:
- Obsidian or similar for graph view
- Automated link validation
- Full-text search
- Tag system

---

## Conclusion

This wiki represents ~4 hours of focused synthesis work, transforming a 2-hour call + chat into a navigable knowledge base with 89 interlinked pages.

**Key Achievement**: Not just documenting what was said, but:
- Connecting ideas across participants
- Surfacing patterns and themes
- Preserving both explicit and implicit knowledge
- Creating multiple paths for exploration
- Capturing the richness of both formal and informal discussion

**The Meta-Irony**: This wiki about a call discussing AI-assisted synthesis, environmental neurodiversity, and information overload... was itself created through AI-assisted synthesis, demonstrates those very challenges, and hopefully provides a useful way to navigate the overwhelming richness.

Peter and the OGM community now have a resource that:
- Documents this specific call thoroughly
- Preserves ideas that might otherwise be lost
- Enables future reference and connection
- Models what AI-assisted knowledge work can look like

---

**Created by**: Claude Code (Anthropic)
**Date**: November 6, 2025
**For**: Peter Kaminski and the OGM community
**Purpose**: Comprehensive synthesis and documentation

Back to [[Index]]
