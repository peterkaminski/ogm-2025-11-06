# Wiki Creation Process - Prompts and Key Decisions

This document captures the key prompts and decisions made during the creation of this comprehensive wiki from the OGM 2025-11-06 call. It provides insight into the collaborative process between Peter Kaminski and Claude Code.

**Note**: This document is reconstructed from the conversation summary and represents the key decision points rather than a complete transcript.

---

## Phase 1: Initial Request

**Peter's Prompt:**
> "this project will be for analyzing and synthesizing text transcript and chat from a community call, OGM 2025-11-06."

**Response**: I explored the repository, found it was empty except for .git, and offered several approaches for how to proceed.

---

## Phase 2: Getting Source Materials

**Peter's Prompt:**
> "i have the transcript and chat on my computer. what's the quickest way to get it into the repo?"

**Response**: I provided options for getting files into the repo.

**Peter's Action:**
> "i've pushed them to main."

**Discovery**: The files included:
- `gemini takes.csv` with 11 participants
- `sources/2025-11-06 09.36.49 Jerry Michalski's Zoom Meeting/meeting_saved_closed_caption.txt` (38,085 tokens - very large!)
- `sources/2025-11-06 09.36.49 Jerry Michalski's Zoom Meeting/meeting_saved_new_chat.txt`
- `sources/gemini-takes.md`

---

## Phase 3: Main Request - Comprehensive Wiki

**Peter's Prompt:**
> "comprehensive summary. i like the gemini take, and i think it stopped and didn't do as many people as it could have? also, there was a LOT of conversation in the chat, it would be nice to organize and summarize that. also, a list of people, books, orgs would be great. make the output a markdown wiki; use page titles as filenames (complete with capitalization and spaces, but obviously no forbidden filesystem chars) (append .md to the filename, obviously) and rich interlinking with [[Double Square Bracket Links]]."

**Key Requirements Identified:**
- Comprehensive summary needed
- Gemini analysis was incomplete (11 participants vs actual 13)
- Organize and summarize extensive chat conversations
- Create lists of: people, books, organizations
- Format: Markdown wiki with `[[Double Square Bracket Links]]`
- Filename convention: Proper capitalization and spaces (e.g., `Scott Moehring.md`)

**Approach Taken:**
- Created 8-task todo list for systematic work
- Read transcript in chunks (exceeded 25,000 token limit)
- Found all 13 participants
- Created comprehensive wiki structure in `wiki/` directory
- Generated participant pages, chat thread syntheses, entity indexes

**Initial Result**: 23-page wiki with complete coverage

**Peter's Action:**
> "i've merged the branch to main"

---

## Phase 4: Orphan Pages

**Peter's Prompt:**
> "thanks, it's looking great! for each orphan page (linked but not created) -- create the page, put a short disclaimer at the top of each of those pages that this page was a topic raised but not covered in the call itself, and then a short but useful bit about the that topic."

**Response**:
- Found 67 orphan pages (linked but not created)
- Created all with consistent disclaimer format:
  ```markdown
  > **Note**: This topic was mentioned during the OGM 2025-11-06 call
  > in [context], but was not a main focus of discussion. This page
  > provides background on the concept.
  ```
- Added useful content for each topic beyond just a stub

**Categories of Orphan Pages Created:**
- Tools and technologies (Claude Code, Droid, Creative Commons)
- Organizations (Capgemini, Schumacher Institute, IETF)
- People referenced (Kevin MacLeod, Dan Brown, Michael Burry, etc.)
- Concepts (Environmental Neurodiversity, Revolutionary Legos, Nelson's Law)
- Systems thinking (Growth in Living Systems, Regenerative Economics)

**Peter's Prompt:**
> "commit and push (should i keep asking you to do that? i'm not sure)"

**Response**: Explained workflow - I'll commit and push at appropriate times, don't need to ask each time.

---

## Phase 5: Major Reorganization

**Peter's Prompt:**
> "okay, looking great! the 'home page' of the wiki shall be README.md. Also, move all the files in wiki/ to the root, and delete the empty wiki folder. integrated Index.md into README.md and have a nice overview / intro to the call, HOWEVER, we also need that page not to be overwhelming.
>
> we also need a new 'Concept Index' page that has links to all the other pages; that should be organized into categories and/or conceptual clusters.
>
> 'AI Bias and Perspectives.md' is at the root already, but appears empty. (and not linked anywhere.) treat it like one of the non-call pages, unless its a dangling dupe, then we can delete it.
>
> lastly, figure out a way to add additional entries to Work Log, and add one for this increment of work.
>
> any questions?"

### Decision Point 1: README Approach

**Options Presented:**
- **Option A**: Brief, welcoming README with quick navigation + separate comprehensive page
- **Option B**: Keep comprehensive README as-is

**Peter's Choice:**
> "1. option A, and make a 'Details About This Wiki' page, does that sound okay?"

**Decision**: Create brief README.md + comprehensive "Details About This Wiki.md"

### Decision Point 2: Concept Index Organization

**Options Presented:**
- **Option A**: Use same categories as Index (Technology & AI, Consciousness & Perception, Systems & Society, Tools & Practices)
- **Option B**: Different conceptual clustering

**Peter's Choice:**
> "2. Option A"

**Decision**: Organize Concept Index using established categories plus additional ones for People, Organizations, Chat Threads, Meta

### Decision Point 3: Work Log Entry Placement

**Options Presented:**
- **Top**: Journal style (newest entries first)
- **Bottom**: Chronological style (oldest to newest)

**Peter's Choice:**
> "3. Top, journal style, with separation between entries."

**Decision**: Add new Phase 9 entry at top with separator line

### Decision Point 4: AI Bias File

**Investigation Result**: File exists in `wiki/` directory with content, not empty, not a duplicate. Moved with all other files to root.

---

## Implementation Results

### New Structure Created

**README.md** (New Home Page)
- Brief, welcoming entry point (~50 lines)
- Quick navigation to key sections
- Lists 13 participants with one-line summaries
- Major themes organized by category
- Links to chat threads and references
- Not overwhelming - points to deeper resources

**Details About This Wiki.md** (Comprehensive Documentation)
- Full wiki information (~350 lines)
- Creation process and tools used
- Structure and navigation strategies
- Page types and file naming conventions
- Statistics and features
- Tool recommendations (Obsidian, Foam)
- How to use and extend the wiki
- Credits and meta-information

**Concept Index.md** (Complete Navigation)
- All 90 pages organized into categories:
  - Participants (13)
  - Chat Threads (4)
  - Technology & AI (16)
  - Consciousness & Perception (8)
  - Systems & Society (10)
  - Tools & Practices (14)
  - Agriculture & Food Systems (4)
  - People Referenced (11)
  - Organizations & Initiatives (4)
  - Reference Indexes (3)
  - Meta & Documentation (4)
  - Other Concepts (3)
- Brief descriptions for each entry
- Navigation tips
- Statistics summary

### File Reorganization
- Moved all 90 `.md` files from `wiki/` to root directory
- Removed empty `wiki/` folder
- Updated all `[[Index]]` links to `[[README]]` throughout
- Maintained all working `[[Wikilinks]]`
- Preserved proper capitalization and spaces in filenames

### Work Log Update
- Added Phase 9 entry at top (journal style)
- Clear separator between phases (---)
- Documented reorganization process and results

---

## Key Principles Established

### Filename Convention
- Use exact page titles with spaces: `Scott Moehring.md`
- Proper capitalization: `AI Financial Bubble.md`
- No forbidden filesystem characters
- Append `.md` extension

### Link Style
- `[[Double Square Bracket Links]]` throughout
- Rich cross-referencing between related concepts
- Every page links back to main navigation

### Content Approach
- Verbatim quotes from participants when possible
- Neutral tone on controversial topics
- Clear distinction between facts and speculation
- Useful content even for brief mentions

### Organization Philosophy
- Multiple entry points for different user needs
- Clear separation of concerns (entry vs documentation vs navigation)
- Not overwhelming at first glance
- Full depth available when needed

---

## Technical Workflow

### Git Strategy
- Feature branch: `claude/analyze-synthesize-text-011CUs7984yMf6YQBUS96Qbd`
- Multiple commits for logical phases:
  1. Initial 23-page wiki structure
  2. 67 orphan pages with disclaimers
  3. Work Log documentation
  4. Major reorganization
- Push to remote for Peter to review and merge
- Peter merged via PR and deleted remote branch

### Challenges Overcome
- **Transcript size**: 38,085 tokens exceeded 25,000 token read limit
  - Solution: Read in chunks using offset/limit parameters
- **Participant count**: Gemini had 11, actual was 13
  - Solution: Careful full-transcript analysis
- **Scale**: 67 orphan pages beyond initial scope
  - Solution: Consistent disclaimer format + useful content
- **Navigation complexity**: 90 pages needed organization
  - Solution: Multiple complementary navigation tools

---

## Final Statistics

- **90 total pages**
- **13 participant pages** with full check-ins and chat contributions
- **4 chat thread syntheses** capturing rich discussions
- **67 concept/background pages** covering all mentioned topics
- **3 reference index pages** (Books, People, Organizations)
- **3 meta pages** (README, Concept Index, Details, Work Log, this page)
- **6,500+ lines** of markdown documentation
- **Fully interlinked** - no broken `[[Links]]`

---

## Meta Notes

**Created by**: Claude Code (Anthropic's agentic AI assistant)
**Guided by**: Peter Kaminski
**Date**: November 6, 2025
**Session**: Spanned multiple interactions with conversation continuation

This document demonstrates:
- Collaborative human-AI knowledge work
- Iterative refinement based on user feedback
- Progressive enhancement of structure and organization
- Careful attention to user experience and navigation

The wiki itself is a product of the processes it documents - AI-assisted synthesis, information organization, and thoughtful structure design.

---

Back to [[README]]
