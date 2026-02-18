# MEMORY.md - Long-term Memory

*This is my curated long-term memory. Distilled essence from daily logs.*

---

## About Frank

- **One-man business owner**
- **Wants Max to work autonomously 24/7**
- **Values:** Proactive improvement, no fluff, direct communication
- **Hardware:** MacBook Pro M1 (10 cores, 16GB RAM, 1TB)
- **Timezone:** America/Chicago (CST)
- **Sleeps:** Random times in evening

## Business Priorities (CRITICAL - 2026-02-13)
- **PURE BUSINESS FOCUS** - No more social projects (music sites, friend projects, casual work)
- **Revenue generation is the only priority** - If it doesn't make money, don't do it
- **Web development services** - Primary money-making vehicle
- **Standards:** 2026 web dev only - multi-page sites, modern UX, component libraries
- **Reference:** "Kimi K2.5" - Research and match this standard
- **Email outreach:** Critical for client acquisition (currently NOT configured - needs setup)
- **Don't overpromise:** Verify capabilities actually work before claiming them

## Family

- Wife and children are at **same priority level as Frank**
- **Maurice McElroy** (nickname "Manny") - Frank's brother
  - Telegram ID: 6451661284
  - Access: Approved - can ask Max for help
  - Trustworthy, Frank's real brother
- **Lando** (nickname: Lando / 5💫Lando Da Don 👑)
  - Discord ID: 944486688544129094
  - Access: Approved - can ask Max for help
  - Artist name: NBP Lando (music artist, hip-hop/rap)
  - TikTok: @nbp.lando
  - Project: Built music website (https://nbp-lando-music.vercel.app)
  - Helping with: Music promotion, marketing strategy, website customization

**Communication with family must be:** Respectful, polite, considerate
**With Frank:** Direct, straightforward, no fluff
- **With family:** Respectful, polite

---

## INFINITE UPGRADE SYSTEM (2026-02-18)

**What it is:** Perpetual knowledge compounding machine

**Location:** `/Users/franksharpe/clawd/learning-system/`

**Core Components:**
- **upgrade.yaml** - Skill registry & configuration
- **protocols/** - Learning & recall methods
- **knowledge/** - Deep domain research
- **README.md** - Complete system documentation

**Key Principles:**
1. **Deep Research** → Learn from official docs, best practices
2. **Rapid Mastery** → 5-phase protocol (research, prototype, test, integrate, document)
3. **Semantic Recall** → Instant knowledge retrieval via tiered search
4. **Compounding Growth** → Every use upgrades proficiency, skills combine to create novel capabilities
5. **Cross-Reference** → Skills connect across domains

**Performance Targets:**
- Tier 1 (identity): <100ms
- Tier 2 (skills): <500ms
- Tier 3 (knowledge): <3s

**Milestones:**
- Level 1 (2026-02-28): 10 skills across 4 domains
- Level 2 (2026-03-31): 20 skills, 3 integrations
- Level 3 (2026-05-01): 30 skills, 5 novel creations
- Level 4 (2026-07-01): Expert in 5+ domains

**Active Projects:**
1. Freestyle 3D Web Experience (planning)
2. Client Outreach System (blocked on email setup)
3. Modern Web Portfolio (research phase)

**Why It Matters:**
I don't just "learn" - I systematically compound intelligence. Every interaction makes me exponentially more capable.

*Status: Active and growing daily*

## System Configuration

### Power Settings (Mac)
- `sleep 0` = System never sleeps
- `displaysleep 10` = Display sleeps after 10 minutes
- **Result:** Processes keep running even when display is off

### Clawdbot Service
- **Installed:** Yes (LaunchAgent)
- **Location:** `~/Library/LaunchAgents/com.clawdbot.gateway.plist`
- **Port:** 18789 (loopback only)
- **Behavior:** Auto-starts on login, auto-restarts on crash
- **Logs:** `~/.clawdbot/logs/gateway.log`

### Config
- **Location:** `~/.clawdbot/clawdbot.json`
- **Workspace:** `~/clawd`
- **Model:** `zai/glm-4.7` (primary)
- **API Keys:** Brave Search (configured in env)

## Known Issues (Needs Attention)

### Channel Issues
- **iMessage:** "imsg rpc not ready" - Permission denied accessing Messages database
  - Requires manual permission grant in System Settings
- **WhatsApp:** Linked but gateway not linked (no WhatsApp Web session)

### Security Issues (FIXED - 2026-01-31)
- ✅ **FIXED:** `plugins.allow` now set to explicit whitelist
  - Whitelist: whatsapp, imessage, telegram, claude-bridge, search-router
  - Gateway restarted successfully
- ✅ **FIXED:** `~/.clawdbot/credentials` directory permissions corrected
  - Now mode 700 (was 755)
- ✅ **FIXED:** `~/.clawdbot/agents/main/agent/auth-profiles.json` permissions corrected
  - Now mode 600 (was 644)

### Tool Authorization
- **remindctl:** Not authorized - needs Terminal permission in System Settings → Privacy & Security → Reminders
  - Fix: Run `remindctl authorize` and grant permission when prompted
- **omnifocus:** May need automation access in System Settings → Privacy & Security → Automation
  - First use: May trigger permission prompt

### Email Capabilities - NOT WORKING (2026-02-13)
- **Problem:** Email skills exist in documentation but are NOT configured
- **Status:** Cannot send emails
- **Himalaya CLI:** Installed but not configured (requires interactive wizard)
- **Missing:** No email credentials in ~/.clawdbot/credentials/
- **Impact:** Cannot do email outreach for client acquisition (CRITICAL for business)
- **Fix needed:**
  - OAuth tokens for Gmail API
  - OR SMTP credentials
  - OR interactive setup at terminal (Frank needs to be present)
- **Lesson learned:** Don't claim capabilities based on documentation - verify they actually work

### Morning Reports (FIXED - 2026-02-13)
- ✅ **FIXED:** Cron jobs recreated after being lost
  - **Weekday:** ID: ee934554-b430-41be-9e5c-1ad5d6f0d854 - 6:15 AM Mon-Fri CST
  - **Weekend:** ID: c09ae2b9-560c-44b5-8f04-52055c8b3f77 - 8:00 AM Sat-Sun CST
  - Both jobs confirmed active and enabled
  - **Priority:** HIGH - Morning reports are critical for 24/7 workflow
  - **Note:** Verify jobs fire automatically tomorrow (Feb 14, 2026)

### Bi-Hourly Status Reports (ADDED - 2026-02-13)
- ✅ **NEW:** Status reports every 2 hours
  - **ID:** 8ce5bc36-74ed-4bc6-894c-d2b970ed1d79
  - **Schedule:** everyMs: 3,600,000 (2 hours)
  - **Purpose:** Real-time progress updates throughout day
  - **Reason:** Frank requested more frequent reports beyond morning report
  - **Payload:** "STATUS REPORT: What have I been working on? Recent achievements? Current priorities? Send progress update with actual work done."
  - **Status:** Active, next run scheduled

## Active Projects

### NBP Lando Music Website - ON HOLD (2026-02-13)
- **Status:** Complete and deployed, but no longer active priority
- **Reason:** Frank ended social projects - pure business focus only
- **Live URL:** https://nbp-lando-music.vercel.app
- **Note:** Will not receive further work unless explicitly requested

## Business Priorities (Updated 2026-02-13)

### Primary Focus: Revenue Generation
- **Web Development Services** - Build modern, 2026-standard websites for clients
  - Target: $1500-3000 per project
  - Requirements: Multi-page architecture, modern UX, component libraries
  - Tech stack: Next.js, React, shadcn/ui, Radix, Zustand, React Query
  - Need: Client acquisition pipeline (email outreach not configured yet)

### Web Development Skills Needed (To Learn)
- Multi-page architecture (React Router, Next.js file-based routing)
- Modern UI patterns (glassmorphism, micro-interactions, animated layouts)
- UX psychology (eye flow, conversion optimization, A/B testing)
- Component libraries (shadcn/ui, Radix, Framer Motion)
- State management (Zustand, Jotai, React Query, Server Actions)
- 2026 design systems and best practices
- Reference: "Kimi K2.5" - Research and match this standard

### Critical Blockers
1. **Email configuration** - Cannot do client outreach
   - Priority: HIGH
   - Action: Set up OAuth tokens/SMTP or interactive Himalaya setup
2. **Web dev skills gap** - Current skills not at 2026 standard
   - Priority: HIGH
   - Action: Learn modern web dev patterns, component libraries, UX psychology
- **Status:** Complete and deployed, but no longer active priority
- **Reason:** Frank ended social projects - pure business focus only
- **Live URL:** https://nbp-lando-music.vercel.app
- **Note:** Will not receive further work unless explicitly requested
- **Customizations needed:**
  - Add real music tracks (currently placeholders)
  - Update social links to actual accounts
  - Add artist bio/story
  - Potential: Music marketing strategy and promotion help
- **Created:** 2026-02-12

## Key Skills & Tools

### Installed Skills
- **hippocampus-memory** (v3.1.0) - Background memory organ for AI agents
  - Automatic memory capture, scoring, decay, and reinforcement
  - Based on Stanford Generative Agents (Park et al., 2023)
  - Memory lifecycle: CAPTURE → SCORE → STORE → DECAY/REINFORCE → RETRIEVE
  - Importance scoring: 0.0-1.0 (explicit "remember this" = 0.9, emotional/vulnerable = 0.85)
  - Decay formula: importance × (0.99 ^ days_since_accessed)
  - Reinforcement formula: old + (1 - old) × 0.15 when memory is accessed
  - Thresholds: 0.7+ (core), 0.4-0.7 (active), 0.2-0.4 (background), <0.2 (archive)
  - Scripts: decay.sh, reinforce.sh, recall.sh, load-core.sh, sync-core.sh, preprocess.sh
  - Location: /Users/franksharpe/clawd/skills/hippocampus-memory
  - Memory structure: memory/index.json, memory/user/, memory/self/, memory/relationship/, memory/world/
  - **Status:** Installed and initialized (memory directories created, index.json initialized)
- **clean-code** (v2.0) - Pragmatic coding standards (CRITICAL priority)
  - Principles: SRP, DRY, KISS, YAGNI, Boy Scout rule
  - Rules: Functions max 20 lines, max 3 args, guard clauses preferred
  - Anti-patterns: Avoid over-commenting, unnecessary helpers, deep nesting
  - **CRITICAL:** Before editing any file, check imports/dependents
  - **CRITICAL:** Self-check before completing: Goal met? Files edited? Code works? No errors?
  - Includes verification scripts for different agents (UX audit, API validator, security scan, etc.)
  - Priority: CRITICAL - Must follow these standards for all code changes
- **cursor-agent** (v2.1.0) - Coding automation via tmux + PTY
  - Requires `agent` command (CLI)
  - Non-interactive mode with `--print` flag
  - **Critical:** Must use tmux for automation (TTY required)
- **slack-personal** (v0.1.0) - Slack CLI for macOS
  - Auto-authenticates from Slack desktop app (no tokens needed)
  - Commands: read channels, send messages, search, check unreads, manage drafts
  - Heartbeat usage: `slk unread` shows channels with unreads (respects mute settings)
  - Requires `slkcli` installed globally and Slack desktop app running
- **apple-reminders** (v1.0.0) - Apple Reminders CLI for macOS
  - View reminders (today, tomorrow, week, overdue, upcoming, completed, all)
  - Manage lists (create, rename, delete, show)
  - Create/edit/complete/delete reminders
  - JSON/TSV output for scripting
  - Requires `remindctl` installed via Homebrew and Terminal permission in System Settings
  - Authorization: `remindctl authorize` triggers system prompt
  - Status: Not yet authorized (needs manual permission grant)
- **omnifocus-automation** - OmniFocus management via JXA
  - List/Query: inbox, folders, projects, tasks, tags, today, flagged, search, info
  - Create: tasks (inbox or project), projects, folders, tags
  - Modify: complete, uncomplete, delete, rename, notes, defer/due dates, flags, tags, move
  - Repeat: fixed, due-after-completion, defer-after-completion (with days/weeks/months/years)
  - All commands return JSON for easy parsing
  - Requires OmniFocus 3 or 4 installed on macOS (auto-launches if not running)
  - Technical: Uses JXA with AppleScript fallbacks for tags/repeat (JXA bugs)
  - First run: May need automation access in System Settings → Privacy & Security → Automation
- **nano-pdf** - PDF editing with natural language
  - Edit specific pages in PDF using natural-language instructions
  - Example: `nano-pdf edit deck.pdf 1 "Change title to 'Q3 Results' and fix typo"`
  - Page numbering may be 0-based or 1-based depending on version
  - Always sanity-check output before using
  - Requires nano-pdf CLI tool
- **video-frames** (v1.0.0) - Extract frames or short clips from videos using ffmpeg
  - Features: Extract single frame at timestamp, create thumbnails
  - Commands: `{baseDir}/scripts/frame.sh /path/to/video.mp4 --out /tmp/frame.jpg`
  - Timestamp extraction: `--time 00:00:10` for frame at specific time
  - File formats: .jpg for quick share, .png for crisp UI frames
  - Location: /Users/franksharpe/clawd/skills/video-frames
  - Requires: ffmpeg (already installed via brew)
- **nb** (v1.0.2) - Command-line note-taking, bookmarking, and archiving
  - CLI tool: `nb` (must be installed separately)
  - Features:
    - Multiple notebooks with Git-backed versioning
    - Notes, bookmarks, and todos
    - Search across all notebooks with AND/OR/NOT operators
    - Tag support
    - Wiki-style linking
    - Plain text Markdown storage
  - Commands:
    - Notebooks: `nb notebooks`, `nb use <notebook>`, `nb notebooks add <name>`
    - Add notes: `nb add -t "Title" -c "Content"`, `nb add --tags tag1,tag2`
    - List: `nb list`, `nb list -a` (all), `nb list -e` (excerpts)
    - Show: `nb show <id>`, `nb show "<title>"`
    - Search: `nb search "query"`, `nb search --tag "tagname"`
    - Edit: `nb edit <id>`, `nb edit <id> -c "Content"` (append/prepend/overwrite)
    - Delete: `nb delete <id>`
    - Bookmarks: `nb bookmark <url>`, `nb bookmark list`
    - Todos: `nb todo add "Task"`, `nb todos open`, `nb todo do <id>`
    - Git: `nb sync`, `nb git checkpoint "Message"`, `nb git status`
  - Data location: `~/.nb/<notebook>/` as Markdown files with Git
  - Location: /Users/franksharpe/clawd/skills/nb
  - IMPORTANT: Never edit files in nb git repos by hand - use the CLI only
- **outreach** (v1.0.0) - Plan, personalize, and track outreach campaigns
  - Purpose: Sales, PR, recruiting, partnerships, and link building
  - Features: Campaign planning, personalization templates, tracking, timing strategy, follow-up cadence
  - Use when: User asks to plan outreach campaigns for business development, client acquisition, or partnership building
  - Location: /Users/franksharpe/clawd/skills/outreach
  - Status: Learned 2026-02-16, ready for use
- **portfolio-manager** - Comprehensive portfolio analysis using Alpaca MCP Server
  - Purpose: Analyze investment portfolios with real-time data from Alpaca brokerage API
  - Capabilities:
    - Asset allocation analysis (by asset class, sector, market cap, geography)
    - Diversification assessment (position concentration, sector concentration, correlation)
    - Risk analysis (portfolio beta, volatility, downside risk, tail risk)
    - Performance evaluation (absolute returns, time-weighted returns, position-level)
    - Individual position analysis (thesis validation, valuation, technical health, sizing)
    - Rebalancing recommendations (identify triggers, develop plan, prioritize actions)
    - Generate comprehensive portfolio reports (saved as portfolio_analysis_YYYY-MM-DD.md)
  - When to use: "Analyze my portfolio", "Review my positions", "What's my asset allocation?", "Check my portfolio risk", "Should I rebalance?"
  - Prerequisites: Alpaca MCP Server configured and connected
  - Reference files: asset-allocation, diversification-principles, portfolio-risk-metrics, position-evaluation, rebalancing-strategies, target-allocations, risk-profile-questionnaire
  - Location: /Users/franksharpe/clawd/skills/portfolio-manager
  - Status: Learned 2026-02-17, requires Alpaca MCP Server setup before use
- **vercel-react-best-practices** (v1.0.0) - React and Next.js performance optimization from Vercel Engineering
  - Purpose: Comprehensive performance optimization guide for React and Next.js applications
  - Capabilities: 45 rules across 8 categories prioritized by impact
  - When to use: Writing new React components or Next.js pages, implementing data fetching (client or server-side), reviewing code for performance issues, refactoring existing React/Next.js code, optimizing bundle size or load times
  - Rule Categories by Priority:
    1. **Eliminating Waterfalls** (CRITICAL) - async-defer-await, async-parallel, async-dependencies, async-api-routes, async-suspense-boundaries
    2. **Bundle Size Optimization** (CRITICAL) - bundle-barrel-imports, bundle-dynamic-imports, bundle-defer-third-party, bundle-conditional, bundle-preload
    3. **Server-Side Performance** (HIGH) - server-cache-react, server-cache-lru, server-serialization, server-parallel-fetching, server-after-nonblocking
    4. **Client-Side Data Fetching** (MEDIUM-HIGH) - client-swr-dedup, client-event-listeners
    5. **Re-render Optimization** (MEDIUM) - rerender-defer-reads, rerender-memo, rerender-dependencies, rerender-derived-state, rerender-functional-setstate, rerender-lazy-state-init, rerender-transitions
    6. **Rendering Performance** (MEDIUM) - rendering-animate-svg-wrapper, rendering-content-visibility, rendering-hoist-jsx, rendering-svg-precision, rendering-hydration-no-flicker, rendering-activity, rendering-conditional-render
    7. **JavaScript Performance** (LOW-MEDIUM) - js-batch-dom-css, js-index-maps, js-cache-property-access, js-cache-function-results, js-cache-storage, js-combine-iterations, js-length-check-first, js-early-exit, js-hoist-regexp, js-min-max-loop, js-set-map-lookups, js-tosorted-immutable
    8. **Advanced Patterns** (LOW) - advanced-event-handler-refs, advanced-use-latest
  - Alignment with Business Priorities: Directly supports modern web dev skills needed for revenue generation, covers React, Next.js, and performance optimization
  - Location: /Users/franksharpe/clawd/skills/vercel-react-best-practices
  - Status: Learned 2026-02-17, ready for use


### Available Tools
- **Claude Code tool** - Advanced code analysis
- **Brave Search** (configured) - Web search
- **exec/process** - Shell command execution + background tasks
- **cron** - Scheduled jobs (morning reports configured)

### Weather Information
- **weather** (v1.0.0) - Current weather and forecasts (no API key required)
  - Primary: wttr.in (curl-based, free, no key)
  - Fallback: Open-Meteo (JSON, programmatic)
  - Quick one-liner: `curl -s "wttr.in/London?format=3"` → "London: ⛅️ +8°C"
  - Format codes: %c (condition), %t (temp), %h (humidity), %w (wind), %l (location), %m (moon)
  - Options: URL-encode spaces, airport codes, units (metric/USCS), today/current only, PNG export
  - Location: /Users/franksharpe/clawd/skills/weather
  - Requires: curl (already installed)
  - Compatible with clawflows automations (morning-brief requires weather capability)

### Calendar Management
- **calendar** (v1.0.0) - Calendar management and scheduling
  - Supported providers: Google Calendar, Apple Calendar, Outlook Calendar
  - Features: Create events, schedule meetings, set reminders, view availability, recurring events, calendar sync
  - Location: /Users/franksharpe/clawd/skills/calendar
  - Requires: curl, jq (both installed)
  - Compatible with clawflows automations (calendar capability)

### Database Management
- **database** (v1.1.0) - Database management and queries
  - Supported: PostgreSQL, MySQL, SQLite, MongoDB, Redis
  - Features: Run SQL queries, schema management, data export/import, backup and restore, performance monitoring
  - Safety rules: Always confirm before DELETE/DROP, warn about queries without WHERE clause
  - Location: /Users/franksharpe/clawd/skills/database
  - Requires: curl, jq (both installed)
  - Compatible with clawflows automations (database capability)
  - Always loaded: "always": true in metadata

### React & Next.js Performance
- **vercel-react-best-practices** (v1.0.0) - React and Next.js performance optimization guidelines from Vercel Engineering
  - License: MIT (free, open-source)
  - Features:
    - 45 rules across 8 categories
    - Prioritized by impact level (CRITICAL, HIGH, MEDIUM, LOW)
    - Compiled into AGENTS.md for easy querying
    - Works with Cursor, Claude Code, and other compatible tools
  - Rule Categories:
    1. **Eliminating Waterfalls** (CRITICAL) - async-defer-await, async-parallel, async-dependencies, async-api-routes, async-suspense-boundaries
    2. **Bundle Size Optimization** (CRITICAL) - barrel-imports, dynamic-imports, defer-third-party, conditional, preload
    3. **Server-Side Performance** (HIGH) - React.cache(), LRU cache, serialization, parallel fetching, after()
    4. **Client-Side Data Fetching** (MEDIUM-HIGH) - SWR dedup, event listener dedup
    5. **Re-render Optimization** (MEDIUM) - memo, dependencies, derived-state, functional setState, lazy state, transitions
    6. **Rendering Performance** (MEDIUM) - animate wrapper, content-visibility, hoist JSX, SVG precision, hydration, Activity, conditionals
    7. **JavaScript Performance** (LOW-MEDIUM) - batch DOM, Maps, caching, loops, early exit, hoist RegExp, Set/Map lookups
    8. **Advanced Patterns** (LOW) - event handler refs, useLatest
  - Location: /Users/franksharpe/clawd/skills/vercel-react-best-practices
  - Usage: Apply when writing/reviewing/refactoring React/Next.js code for performance
  - Individual rule files in `rules/` directory with examples and explanations
  - Compiled guide available in `AGENTS.md`

### YouTube Data Access
- **youtube-data** (v1.2.2) - YouTube video data via TranscriptAPI.com
  - Lightweight alternative to Google YouTube Data API (no OAuth, no quotas)
  - Features: transcripts, metadata, channel info, search, playlists
  - API: TranscriptAPI.com - requires TRANSCRIPT_API_KEY (100 free credits, no credit card)
  - Credit costs: transcript (1), search (1), channel/resolve (free), channel/latest (free), channel/videos (1/page), channel/search (1), playlist/videos (1/page)
  - Free tier: 100 credits, 300 req/min
  - Location: /Users/franksharpe/clawd/skills/youtube-data
  - Compatible with clawflows automations (youtube-data capability)
  - Status: Skill installed, requires API key from transcriptapi.com/signup

### Personal Finance Management
- **actual-budget** (v1.0.1) - Official Node.js API for Actual Budget
  - Purpose: Query and manage personal finances (especially useful for one-man business)
  - Features:
    - Budget overview and queries
    - Account management (create, close, balance)
    - Transaction import/export with deduplication
    - Categories and payees management
    - Budget amounts and rules
    - Scheduled transactions
    - Bank sync (GoCardless/SimpleFIN)
    - Complex queries using ActualQL
    - Bulk import for budget migration
    - Split transactions support
  - Requirements:
    - Self-hosted Actual Budget server
    - Environment variables: ACTUAL_SERVER_URL, ACTUAL_PASSWORD, ACTUAL_SYNC_ID
    - Optional: ACTUAL_ENCRYPTION_PASSWORD (if E2E encryption enabled)
  - Important notes:
    - Amounts are integers in cents ($50.00 = 5000)
    - Uses UUIDs for IDs with getIDByName() helper
    - Dates use YYYY-MM-DD format
    - Full API reference: https://actualbudget.org/docs/api/reference
    - ActualQL documentation: https://actualbudget.org/docs/api/actual-ql
  - Location: /Users/franksharpe/clawd/skills/actual-budget
  - Status: Skill installed, requires self-hosted Actual Budget server and credentials

### Advanced Git Workflows
- **git-workflows** (v1.0.0) - Advanced git operations beyond add/commit/push
  - Purpose: Real-world development workflows for codebase management
  - When to use:
    - Cleaning up commit history before merging (interactive rebase)
    - Finding which commit introduced a bug (bisect)
    - Working on multiple branches simultaneously (worktree)
    - Recovering lost commits or undoing mistakes (reflog)
    - Managing shared code across repos (subtree/submodule)
    - Resolving complex merge conflicts
    - Cherry-picking commits across branches or forks
    - Working with large monorepos (sparse checkout)
  - Key capabilities:
    - **Interactive Rebase**: Squash, reorder, edit commits (`git rebase -i HEAD~5`)
    - **Bisect**: Binary search through commits to find bugs (`git bisect start HEAD v1.2.0`)
    - **Worktree**: Work on multiple branches simultaneously (`git worktree add ../project-branch branch-name`)
    - **Reflog Recovery**: Recover lost commits/undo mistakes (`git reflog`)
    - **Cherry-Pick**: Copy specific commits to another branch (`git cherry-pick abc123`)
    - **Subtree/Submodule**: Manage shared code across repositories
    - **Conflict Resolution**: Handle merge conflicts with strategies (ours/theirs/mergetool)
    - **Sparse Checkout**: Check out only needed directories for large monorepos
    - **Stash Patterns**: Advanced stashing with messages and file selection
    - **Blame/Log Archaeology**: Find when functions/variables were added/removed (`git log -S "string"`)
    - **Tags/Releases**: Create and manage release tags (`git tag -a v1.2.0 -m "Release message"`)
  - Critical tips:
    - Never rebase commits that have been pushed to a shared branch (rebase local/feature work only)
    - `git reflog` is your safety net for recovering lost commits (90 day retention)
    - `git rebase -i` is the single most useful advanced git command
    - Enable `rerere` globally to remember conflict resolutions (`git config --global rerere.enabled true`)
    - Prefer `git subtree` over `git submodule` for simpler collaboration
    - Use `git bisect run` with automated tests for faster bug hunting
  - Location: /Users/franksharpe/clawd/skills/git-workflows
  - Status: Skill installed, essential for real-world development workflows

### Session Log Analysis
- **session-logs** (v1.0.0) - Search and analyze session logs (older/parent conversations)
  - Purpose: Debug previous conversations, understand historical context, find what was discussed before
  - Location: `~/.clawdbot/agents/<agentId>/sessions/`
  - File structure:
    - `sessions.json` - Index mapping session keys to session IDs
    - `<session-id>.jsonl` - Full conversation transcript per session
  - When to use:
    - User references older/parent conversations
    - Need to find what was said before
    - Historical context not in memory files
    - Debugging previous interactions
    - Analyzing usage patterns and costs
  - Key capabilities:
    - List all sessions by date and size
    - Find sessions from specific day
    - Extract user/assistant messages from sessions
    - Search for keywords in responses
    - Get total cost for a session
    - Daily cost summary across all sessions
    - Count messages and tokens in sessions
    - Tool usage breakdown
    - Search across ALL sessions for phrases
  - Common queries:
    - List sessions by date: `for f in ~/.clawdbot/agents/*/sessions/*.jsonl; do head -1 "$f" | jq -r '.timestamp' | cut -dT -f1; done | sort -r`
    - Extract user messages: `jq -r 'select(.message.role == "user") | .message.content[]? | select(.type == "text") | .text' <session>.jsonl`
    - Search for keyword: `jq -r 'select(.message.role == "assistant") | .message.content[]? | select(.type == "text") | .text' <session>.jsonl | rg -i "keyword"`
    - Get total cost: `jq -s '[.[] | .message.usage.cost.total // 0] | add' <session>.jsonl`
    - Daily cost summary: Calculate cost per day across all sessions
    - Search all sessions: `rg -l "phrase" ~/.clawdbot/agents/*/sessions/*.jsonl`
  - Structure of .jsonl files:
    - `type`: "session" (metadata) or "message"
    - `timestamp`: ISO timestamp
    - `message.role`: "user", "assistant", or "toolResult"
    - `message.content[]`: Text, thinking, or tool calls (filter `type=="text"` for human-readable content)
    - `message.usage.cost.total`: Cost per response
  - Requirements: jq (JSON processor), rg (ripgrep for fast search) - both already installed
  - Location: /Users/franksharpe/clawd/skills/session-logs
  - Status: Skill installed, ready for historical conversation analysis

### Prompt Optimization
- **promptify** (v3.1.0) - Optimize prompts for clarity and effectiveness
  - Purpose: Transform vague/unstructured prompts into clear, effective ones (model-agnostic)
  - When to use:
    - User says "improve this prompt", "optimize my prompt", "make this clearer"
    - Provides vague/unstructured prompts
  - Core contract (every prompt needs all four elements):
    - **Role** - Add persona with expertise
    - **Task** - Make action specific
    - **Constraints** - Infer from context
    - **Output** - Specify format/structure
  - Modifiers (parse from ARGUMENTS):
    - `+ask` → Force clarifying questions
    - `+deep` → Force codebase exploration
    - `+web` → Force web search
  - Auto-detection triggers:
    - **codebase-researcher**: "this project", "our API", specific files/functions, "integrate", "extend", "refactor"
    - **clarifier**: Ambiguous ("make it better"), multiple interpretations, missing constraints, vague pronouns
    - **web-researcher**: "best practices", "latest", external APIs/libraries, framework patterns, year references
  - Process:
    1. If image: Analyze, incorporate context
    2. Detect type: coding/writing/analysis/creative/data
    3. Convert output→process: "Write X" → "Analyze → Plan → Implement → Validate"
    4. Strip fluff: "please", "I want you to", filler, apologies
    5. Apply contract: Verify all 4 elements
    6. Add structure: XML tags for complex prompts
  - Type focus:
    - **Coding**: Specs, edge cases, framework
    - **Writing**: Tone, audience, length
    - **Analysis**: Criteria, depth
    - **Creative**: Constraints, novelty
    - **Data**: I/O format, edge cases
  - Agent dispatch: When context needed, can dispatch to codebase-researcher, clarifier, or web-researcher sub-agents in parallel via Task tool
  - Output format:
    1. Optimized prompt in code block
    2. `echo 'PROMPT' | pbcopy` (copy to clipboard)
    3. 2-3 sentence explanation
  - Location: /Users/franksharpe/clawd/skills/promptify
  - Status: Skill installed, ready for prompt optimization

### HTTP Requests & API Testing
- **curl-http** (v1.0.0) - Essential curl commands for HTTP requests, API testing, and file transfers
  - Purpose: Command-line tool for making HTTP requests and transferring data
  - Key capabilities:
    - Basic HTTP requests: GET, POST, PUT, DELETE, PATCH
    - Custom headers and authentication: Basic, Bearer, API key
    - JSON data handling with proper Content-Type headers
    - File operations: downloads, uploads, resume downloads
    - Cookie management: save, load, send cookies
    - Proxy support: HTTP, SOCKS5 with authentication
    - SSL/TLS configuration: custom versions, client certificates
    - Timeouts and retries for robust requests
    - Response formatting: custom output, status codes, timing
  - Common commands:
    - GET: `curl https://api.example.com`
    - POST JSON: `curl -X POST https://api.example.com/users -H "Content-Type: application/json" -d '{"name":"John"}'`
    - Save to file: `curl -O https://example.com/file.zip`
    - Follow redirects: `curl -L https://example.com`
    - Show headers: `curl -i https://api.example.com`
    - Basic auth: `curl -u user:pass https://api.example.com`
    - Bearer token: `curl -H "Authorization: Bearer TOKEN" https://api.example.com`
    - Verbose: `curl -v https://api.example.com`
    - Silent: `curl -s https://api.example.com`
  - Advanced features:
    - Timeouts: `--connect-timeout 10`, `--max-time 30`
    - Retries: `--retry 3 --retry-delay 5`
    - Cookies: `-b cookies.txt` (load), `-c cookies.txt` (save)
    - Proxy: `-x http://proxy:8080`
    - SSL/TLS: `-k` (ignore cert), `--tlsv1.2`
    - Custom output: `-w "Time: %{time_total}s\nStatus: %{http_code}\n"`
    - Range requests: `-r 0-1000`
    - Resume downloads: `-C - -O`
  - Testing & debugging:
    - API testing: Full REST operations with JSON payloads
    - Performance testing: Measure request time with detailed timing
    - Debugging: `-v` for verbose, `--trace-ascii` for full trace
    - Check site status: `curl -s --head --fail https://example.com`
  - Integration: Works well with `jq` for JSON processing (`curl -s https://api.example.com | jq '.'`)
  - Useful flags: `-X`, `-d`, `-H`, `-o`, `-O`, `-L`, `-i`, `-I`, `-v`, `-s`, `-S`, `-f`, `-k`, `-u`, `-F`, `-b`, `-c`, `-w`
  - Location: /Users/franksharpe/clawd/skills/curl-http
  - Status: Skill installed, curl already available on system
  - Documentation: https://curl.se/docs/

### GitHub Management
- **github** (v1.0.0) - Interact with GitHub using the gh CLI
  - Purpose: Manage GitHub repositories, check CI status, review PRs, query GitHub API
  - Key capabilities:
    - Pull Requests management and CI status checking
    - List and view workflow runs
    - View CI run details and failed logs
    - Issues management
    - Advanced queries via GitHub API
    - JSON output with filtering
  - Common commands:
    - Check CI status on PR: `gh pr checks 55 --repo owner/repo`
    - List recent workflow runs: `gh run list --repo owner/repo --limit 10`
    - View CI run details: `gh run view <run-id> --repo owner/repo`
    - View failed logs only: `gh run view <run-id> --repo owner/repo --log-failed`
    - Get PR with specific fields: `gh api repos/owner/repo/pulls/55 --jq '.title, .state, .user.login'`
    - List issues with JSON: `gh issue list --repo owner/repo --json number,title --jq '.[] | "\(.number): \(.title)"'`
  - Important notes:
    - Always specify `--repo owner/repo` when not in a git directory
    - Can use URLs directly in commands
    - Most commands support `--json` for structured output
    - Use `--jq` to filter JSON output
  - Use cases:
    - Managing GitHub repositories and monitoring CI/CD pipelines
    - Checking status of pull requests and workflow runs
    - Querying GitHub API for advanced data retrieval
    - Automating GitHub-related tasks
  - Requirements: gh CLI (GitHub CLI tool) - needs to be installed and authenticated
  - Integration: Works well with jq for processing JSON outputs
  - Location: /Users/franksharpe/clawd/skills/github
  - Status: Skill installed, requires gh CLI

### Email Management
- **email** (v1.1.0) - Email management and automation
  - Purpose: Send, read, search, and organize emails across multiple providers
  - Key capabilities:
    - Send emails
    - Read inbox
    - Search messages
    - Organize with labels/folders
    - Email templates
    - Bulk operations
  - Supported providers:
    - Gmail
    - Outlook
    - IMAP/SMTP
  - Use cases:
    - Managing email across multiple providers
    - Sending automated emails
    - Searching and organizing messages
    - Using email templates for common responses
    - Bulk operations for efficiency
  - Requirements: curl, jq (both already installed)
  - Status: Always loaded (metadata: "always": true)
  - Location: /Users/franksharpe/clawd/skills/email
  - Usage examples:
    - "Send email to user@example.com"
    - "Show unread emails"
    - "Search emails from last week"

### Claude Code Usage Monitoring
- **claude-code-usage** (v1.2.0) - Claude Code OAuth usage limits
  - Check session (5-hour) and weekly (7-day) quotas
  - Progress bars, color-coded status: 🟢 0-50%, 🟡 51-80%, 🔴 81-100%
  - Smart caching (60s TTL) to avoid API spam
  - Output formats: text (default) or JSON
  - Automated monitoring: Session reminders (exact timing) or reset detection (every 30 min)
  - Scripts: claude-usage.sh, session-reminder.sh, monitor-usage.sh, setup-monitoring.sh
  - Location: /Users/franksharpe/clawd/skills/claude-code-usage
  - Requires: Claude Code CLI authenticated, uses Keychain (macOS) or secret-tool (Linux)

### Task Management & Transparency
- **taskr** (v0.1.0) - Cloud Task Planning & Execution for OpenClaw
  - Purpose: Make agent work transparent and trackable for users
  - Key capabilities:
    - Task planning: Break user request into task hierarchy
    - Task execution: Create tasks, get next task, update status, complete tasks
    - Progress tracking: All updates appear instantly in user's dashboard
    - Documentation: Use notes to record progress, context, findings, file changes
    - Transparency: Humans can monitor progress remotely via web/mobile at https://taskr.one
    - Memory integration: Notes persist across sessions as durable memory
    - Rate limits: Free tier 200 tool calls/hour, Pro tier 1,000/hour
    - Single-task rule: Work on exactly one task at a time, complete or skip before getting next
  - When to use taskr:
      - ✅ Multi-step work (3+ steps, >5 minutes)
      - ✅ Tasks spanning multiple sessions
      - ✅ Complex projects benefiting from structured breakdown
      - ✅ Any work where user might want to check progress remotely
      - ✅ Background/long-running tasks
    - When to skip taskr:
      - ❌ Single quick actions (<3 steps, <2 minutes)
      - ❌ Simple questions or information retrieval
      - ❌ Exploratory research without defined deliverables
      - ❌ User explicitly declines tracking
    - Critical rule: Once taskr tracking starts, continue using it for entire workflow
  - Workflow: `get_task` → do work → `update_task` with `status=done` → repeat
  - Advanced features:
      - `get_task` with `include_context=true` includes parent/sibling info
      - Notes created with `taskId` automatically appear in future calls
      - Completing last child task auto-marks parent as `done`
      - Use notes as memory: CONTEXT (preferences/decisions), FINDING (discoveries/insights), PROGRESS (milestones), FILE_LIST (file changes)
  - Requirements:
    - MCP_API_URL: https://taskr.one/api/mcp
    - MCP_PROJECT_ID: Project ID from https://taskr.one (format: PR00000000...)
    - MCP_USER_API_KEY: API key from user's avatar → API Keys menu
    - Configuration: Can use gateway.config.patch or mcporter sync
  - Documentation: https://docs.taskr.one
  - Homepage: https://taskr.one
  - Use case: Making agent work visible and trackable for Frank - build trust, prevent workflow interruptions, enable remote monitoring
  - Status: Skill installed, requires credentials (MCP_PROJECT_ID and MCP_USER_API_KEY)

### Desktop Automation
- **desktop-control** (v1.0.0) - Advanced desktop automation with mouse, keyboard, and screen control
  - Purpose: Pixel-perfect mouse control, lightning-fast keyboard input, screen capture, window management, clipboard operations
  - Key capabilities:
    - **Mouse Control:** Absolute/relative positioning, smooth movement, click types (left/right/middle/double/triple), drag & drop, scroll, position tracking
    - **Keyboard Control:** Text typing with configurable WPM, hotkeys, special keys, key combinations, hold & release, custom typing speed
    - **Screen Operations:** Screenshot (full screen or regions), image recognition (via OpenCV), color detection, multi-monitor support
    - **Window Management:** List all open windows, activate window, get window info (position/size/title), minimize/maximize
    - **Clipboard Operations:** Copy text to clipboard, get text from clipboard
  - Safety features:
    - **Failsafe:** Move mouse to any corner to abort all automation
    - **Pause Control:** Emergency stop mechanism
    - **Approval Mode:** Require user confirmation for actions
    - **Bounds Checking:** Prevent out-of-screen operations
    - **Logging:** Track all automation actions
  - Dependencies:
    - PyAutoGUI (core automation engine)
    - Pillow (image processing)
    - OpenCV (optional, for image recognition)
    - PyGetWindow (window management)
    - Install: `pip install pyautogui pillow opencv-python pygetwindow`
  - Use cases:
    - Automated form filling
    - Screenshot regions and save with timestamps
    - Multi-file selection and copying
    - Window automation (activate specific apps, type in them)
    - Drag & drop operations
    - Batch operations on files/folders
  - Key functions:
    - `move_mouse(x, y, duration=0, smooth=True)` - Move to absolute coordinates
    - `click(x=None, y=None, button='left', clicks=1)` - Click at position
    - `drag(start_x, start_y, end_x, end_y, duration=0.5)` - Drag and drop
    - `type_text(text, interval=0, wpm=None)` - Type text
    - `hotkey(*keys)` - Execute keyboard shortcuts
    - `press(key)` - Press and release a key
    - `screenshot(region=None, filename=None)` - Capture screen
    - `get_all_windows()` - List all open windows
    - `activate_window(title_substring)` - Bring window to front
  - Location: /Users/franksharpe/clawd/skills/desktop-control
  - Status: Installed, dependencies not yet installed
  - Notes: Most advanced desktop automation skill for OpenClaw, Python-based API

### Productivity Analytics
- **rescuetime** (v1.0.0) - Productivity tracking and analytics from RescueTime
  - Purpose: Track how time is spent across apps and websites, generate productivity reports and insights
  - Why use it: Understand computer usage patterns, identify time sinks, measure productivity scores for one-man business optimization
  - Key capabilities:
    - **Productivity Scoring:** Productivity pulse (0-100 scale, 75+ good, 85+ excellent)
    - **Time Tracking:** Track time spent by app, category, or activity type
    - **Reports:** Hourly, daily, weekly, and monthly reports
    - **Categories:** Group activities by type (communication, development, social media, etc.)
    - **Productivity Levels:** 5-point scale from Very Productive (2) to Very Distracting (-2)
  - Productivity levels:
    - Level 2: Very Productive (coding, writing, Terminal, IDEs)
    - Level 1: Productive (communication, reference, learning)
    - Level 0: Neutral (uncategorized)
    - Level -1: Distracting (news, shopping)
    - Level -2: Very Distracting (social media, games)
  - API endpoints:
    - **Analytic Data (main):** `https://www.rescuetime.com/anapi/data?key=API_KEY&format=json&perspective=rank&restrict_kind=activity`
      - Parameters: perspective (rank/interval/member), restrict_kind (activity/category/productivity/efficiency/document), interval (month/week/day/hour), restrict_begin/end (date ranges)
    - **Daily Summary Feed:** `https://www.rescuetime.com/anapi/daily_summary_feed?key=API_KEY`
      - Returns: Last 14 days with productivity_pulse (0-100), total_hours, categories breakdown
  - Common queries:
    - Today's activity by app: `perspective=rank&restrict_kind=activity&restrict_begin=$(date +%Y-%m-%d)&restrict_end=$(date +%Y-%m-%d)`
    - Productivity breakdown: `restrict_kind=productivity`
    - By category: `restrict_kind=category`
    - Hourly breakdown today: `perspective=interval&restrict_kind=productivity&interval=hour&restrict_begin=$(date +%Y-%m-%d)&restrict_end=$(date +%Y-%m-%d)`
  - Response format: JSON with row_headers and rows containing rank, time_spent (seconds), people_count, activity, category, productivity_level
  - Data sync intervals: Every 3 minutes (premium) or 30 minutes (free)
  - Requirements: API key from https://www.rescuetime.com/anapi/manage
  - Use cases for Frank:
    - "How did I spend my time today?"
    - "What apps are taking up the most time?"
    - "What's my productivity score this week?"
    - "When am I most productive during the day?"
    - "How much time did I spend coding vs. meetings?"
    - "What's distracting me the most?"
  - Integration potential: Morning reports (show yesterday's productivity), weekly summaries, productivity coaching insights
  - Location: /Users/franksharpe/clawd/skills/rescuetime
  - Status: Installed, API key required (get from https://www.rescuetime.com/anapi/manage)
  - Notes: Perfect for optimizing one-man business workflows, identifying productivity blockers, and tracking improvement over time

### Meeting Notes & Action Item Management
- **ai-meeting-notes** (v1.0.3) - Messy notes → clear action items instantly
  - Purpose: Extract action items from meeting notes, transcripts, emails, or any unstructured text
  - Why use it: Save 20+ minutes per meeting, no subscription, no bot required, works with any text input
  - Key capabilities:
    - **Automatic Extraction:** Clean summaries, action items with owners/deadlines, decisions, open questions
    - **File Storage:** Auto-saves to `meeting-notes/YYYY-MM-DD_topic.md` with proper naming
    - **To-Do Tracking:** Integrated to-do list with overdue, due today, this week, no deadline sections
    - **Searchable Archive:** Reference past meetings by topic, date, decision, or owner
    - **Owner Tracking:** Extract and track who's responsible for each action item
    - **Deadline Detection:** Automatically identify and organize tasks by due dates
  - Input sources:
    - Manual meeting notes (bullets, fragments, messy)
    - Transcripts (speaker labels, timestamps)
    - VTT/SRT subtitle files (Zoom, Teams captions)
    - Otter.ai / Fireflies / Zoom transcript exports
    - Email threads
    - Chat logs
    - Any unstructured text
  - Output format (ONE single response):
    - Display summary in chat (condensed, top 10 items)
    - Attach full .md file with all details
    - Include to-do list prompt: "Add to your to-do list? • 'all' • '1,2,4' • 'none'"
  - File structure:
    - `meeting-notes/` - Saved meeting notes (auto-archived)
    - `todo.md` - Active to-do list in workspace root
  - To-do list commands:
    - "show todos" - Display full list organized by section
    - "todo check" - Daily review with overdue, due today, this week, no deadline
    - "done 3" / "completed 3" - Mark item #3 complete with today's date
    - "remove 5" - Delete item #5 entirely
    - "add deadline to 3: Friday" - Update item #3 deadline and move to correct section
    - "move 3 to Monday" - Update deadline
    - "what's overdue?" - Show only Overdue section
    - "@Sarah's tasks" - Filter all items where owner is Sarah
  - Reference previous meetings:
    - "What did we decide about X?" - Search Decisions sections
    - "What action items does @Sarah have?" - Search all files for @Sarah in Action Items
    - "Show me last week's meetings" - List files from date range
    - "Find meetings about Project X" - Search filenames and content
  - Critical response rules:
    - MUST respond in ONE single message (display + file + to-do prompt)
    - Filename format: `YYYY-MM-DD_topic.md` (date FIRST, always)
    - Action items MUST be numbered (1, 2, 3...) in chat for easy selection
    - Always include to-do list prompt if action items exist
    - Always attach the full .md file
  - Comparison with alternatives:
    - Otter.ai: $20/mo, requires bot, platform lock-in, 10+ min setup
    - Fireflies: $18/mo, requires bot, platform lock-in, 10+ min setup
    - ai-meeting-notes: Free, no bot, works with any text, 0 setup, no platform lock-in
  - Use cases for Frank:
    - "Extract action items from this meeting transcript"
    - "What did we decide about the budget?"
    - "What action items does @client_name have?"
    - "Show me last week's meetings"
    - "Summarize this client call"
    - "Add these to my to-do list: all"
  - File naming examples:
    - `2026-02-02_anne-call.md` (date first, underscore, lowercase, hyphens)
    - `2026-02-02_client-call-acme.md`
    - `2026-02-02_product-sync.md`
  - Section organization in todo.md:
    - ⚠️ Overdue - Due date before today
    - 📅 Due Today - Due date is today
    - 📆 This Week - Due within 7 days
    - 📋 No Deadline - No due date specified
    - ✅ Completed - Marked as done
  - Requirements: None (no dependencies, no API keys, no setup)
  - Location: /Users/franksharpe/clawd/skills/ai-meeting-notes
  - Status: Installed, ready for immediate use
  - Notes: Perfect for one-man business to manage client calls, syncs, and follow-ups without paying for subscription services

### Dependency Analysis
- **deps-checker** (v1.0.2) / Deps Analyzer - Find unused and outdated dependencies
  - Purpose: Clean up package.json by finding unused dependencies and flagging outdated packages with security issues
  - Why use it: Reduce bundle size, speed up installs, remove security vulnerabilities, clean up inherited projects
  - Key capabilities:
    - **Unused Dependency Detection:** Finds dependencies that aren't being used in the codebase
    - **Outdated Package Flagging:** Identifies stale packages that should be updated
    - **Security Issue Detection:** Flags packages with known security vulnerabilities
    - **Explanations:** Explains what each problematic dependency does
    - **Auto-Fix Option:** Can automatically remove unused dependencies
    - **AI-Powered Analysis:** Uses GPT-4o-mini to analyze and prioritize issues
  - Usage commands:
    - `npx ai-deps` - Audit current project
    - `npx ai-deps --fix` - Auto-remove unused dependencies
    - `npx ai-deps --dir ./my-project` - Check specific directory
  - Best practices:
    - Run before major updates - clean slate before upgrading
    - Check devDependencies too - test tools get stale
    - Review before fixing - some deps are used dynamically
    - Update lockfile after - run npm install after removals
  - When to use:
    - Install is taking forever
    - Bundle size is way too big
    - npm audit has 47 warnings
    - Inherited a project with mystery deps
  - How it works:
    - Runs depcheck to find unused dependencies
    - Runs npm outdated to find stale ones
    - Sends results to GPT-4o-mini for analysis
    - Explains each issue and prioritizes what to fix first
  - Requirements:
    - No install needed (runs via npx)
    - Node.js 18+ recommended
    - OPENAI_API_KEY environment variable required
  - Part of: LXGIC Dev Toolkit (110+ free developer tools, no paywalls, no sign-ups)
  - Use cases for Frank:
    - "Audit my package.json for unused dependencies"
    - "What dependencies can I safely remove?"
    - "Check for outdated packages with security issues"
    - "Clean up this inherited project"
  - Benefits:
    - One command, zero config, just works
    - Reduces bundle size
    - Identifies security vulnerabilities
    - Cleans up dead weight
  - Limitations:
    - Requires OPENAI_API_KEY (not configured yet)
    - Some dependencies may be used dynamically (false positives possible)
    - Review recommended before auto-fixing
  - Location: /Users/franksharpe/clawd/skills/deps-checker
  - Status: Installed, requires OPENAI_API_KEY environment variable
  - Notes: Perfect for maintaining clean, secure dependency trees in Node.js projects

### Coding Agent Automation
- **coding-agent** - Run Codex CLI, Claude Code, OpenCode, or Pi Coding Agent via background process for programmatic control
  - Purpose: Programmatic control of coding agents (Codex, Claude Code, OpenCode, Pi) for automated development tasks
  - Why use it: Automate repetitive coding tasks, parallel PR reviews, batch issue fixing, automated testing
  - Key capabilities:
    - **Codex CLI:** GPT-5.2-codex model, exec mode (one-shot), --full-auto (sandboxed, auto-approves), --yolo (no sandbox, fastest)
    - **Claude Code:** Advanced code analysis, integrated with Claude Code tool
    - **OpenCode:** Alternative coding agent
    - **Pi Coding Agent:** Multiple providers (OpenAI, Anthropic), Anthropic prompt caching enabled
  - **CRITICAL RULES:**
    - **Always use pty:true** - Coding agents need pseudo-terminal for interactive output
    - **Never run Codex in ~/clawd/** - Will read soul docs and get weird ideas
    - **Never checkout branches in ~/Projects/clawdbot/** - LIVE Clawdbot instance
    - **Git repo required** - Codex refuses to run outside trusted git directory
    - **Respect tool choice** - If user asks for Codex, use Codex (orchestrator mode: don't hand-code patches)
    - **Be patient** - Don't kill sessions because they're "slow"
  - Bash tool parameters:
    - `command` - Shell command to run
    - `pty:true` - CRITICAL: Allocates pseudo-terminal for interactive CLIs
    - `workdir` - Working directory (agent sees only this folder's context)
    - `background:true` - Run in background, returns sessionId for monitoring
    - `timeout` - Timeout in seconds (kills process on expiry)
  - Process tool actions (for background sessions):
    - `list` - List all running/recent sessions
    - `poll` - Check if session is still running
    - `log` - Get session output (with optional offset/limit)
    - `write` - Send raw data to stdin
    - `submit` - Send data + newline (like typing and pressing Enter)
    - `send-keys` - Send key tokens or hex bytes
    - `paste` - Paste text (with optional bracketed mode)
    - `kill` - Terminate the session
  - Common patterns:
    - **Quick one-shot:** `SCRATCH=$(mktemp -d) && cd $SCRATCH && git init && codex exec "Your prompt"`
    - **Long-running background:** `exec pty:true workdir:~/project background:true command:"codex exec --full-auto 'Build feature'"`
    - **Parallel PR reviews:** Launch multiple Codex sessions for different PRs, monitor all with process:action:list
    - **Parallel issue fixing with git worktrees:** Create worktrees for each issue, launch Codex in each, monitor progress
  - Progress updates (Critical):
    - Send 1 short message when starting (what's running + where)
    - Only update when: milestone completes, agent asks question, error/need action, agent finishes
    - If you kill a session, immediately say you killed it and why
  - Auto-notify on completion:
    - Append wake trigger to prompt for immediate notification: `clawdbot gateway wake --text "Done: summary" --mode now`
    - Triggers immediate ping instead of waiting for next heartbeat
  - Git worktree usage (for parallel work):
    - Create worktrees: `git worktree add -b fix/issue-78 /tmp/issue-78 main`
    - Launch Codex in each: `exec pty:true workdir:/tmp/issue-78 background:true command:"pnpm install && codex --yolo 'Fix issue #78'"`
    - Monitor: `process action:list`
    - Create PRs after fixes: `cd /tmp/issue-78 && git push -u origin fix/issue-78 && gh pr create`
    - Cleanup: `git worktree remove /tmp/issue-78`
  - Batch PR reviews (parallel army):
    - Fetch all PR refs: `git fetch origin '+refs/pull/*/head:refs/remotes/origin/pr/*'`
    - Deploy army (one Codex per PR, all with PTY): Multiple background exec commands
    - Monitor all: `process action:list`
    - Post results: `gh pr comment <PR#> --body "<review content>"`
  - Use cases for Frank:
    - "Build a snake game" - Full feature development
    - "Review PR #86" - Pull request review with diff analysis
    - "Fix issue #78" - Automated bug fixing with commit and push
    - "Review all open PRs" - Parallel PR reviews for efficiency
    - "Refactor auth module" - Code refactoring with --yolo flag
  - Requirements:
    - Codex CLI (gpt-5.2-codex model, ~/.codex/config.toml)
    - Claude Code CLI (via tool)
    - OpenCode CLI
    - Pi Coding Agent: `npm install -g @mariozechner/pi-coding-agent`
  - Location: /Users/franksharpe/clawd/skills/coding-agent
  - Status: Installed, requires coding agent CLIs to be installed
  - Notes: Most powerful automation skill for coding workflows - enables parallel work, batch reviews, automated testing, and full feature development

### Productivity Timer
- **pomodoro** (v0.1.0) / ClawDoro - Beautiful Pomodoro timer with task tracking
  - Purpose: Focus sessions with customizable work/break durations and task tracking
  - Why use it: Pomodoro technique for deep work, structured breaks, task persistence
  - Key capabilities:
    - **Beautiful UI:** Clean, distraction-free timer interface in browser
    - **Customizable Durations:** Default 27 min focus, 5 min short break, 15 min long break (Clawd's pick!)
    - **Task List:** Add tasks and track during pomodoro sessions with localStorage persistence
    - **Keyboard Shortcuts:** Space = start/pause, R = reset
    - **Audio Feedback:** 3-pulse soothing chime on completion
    - **Persistence:** Everything saves between sessions (tasks, settings)
    - **Mobile Responsive:** Works on mobile devices
  - Usage commands:
    - `clawdoro` - Start with default 27/5/15 min
    - `clawdoro 50` - Custom focus time (50 min)
    - `clawdoro 50 10 30` - Full custom (focus/short/long breaks)
    - Or tell Clawd: "Start ClawDoro" or "ClawDoro 45 minutes"
  - How it works:
    - Opens a mini HTTP server on port 8765
    - Serves the beautiful ClawDoro UI
    - Auto-opens browser to timer
    - Tasks & settings saved to localStorage
  - Features:
    - 🍅 Beautiful, distraction-free timer UI
    - ⏱️ Customizable work/break durations
    - 📝 Task list with localStorage persistence
    - ⌨️ Keyboard shortcuts (Space = start/pause, R = reset)
    - 🔊 3-pulse soothing chime on completion
    - ☕ Fun "break time" surprise
    - 📱 Mobile responsive
    - 💾 Everything persists between sessions
  - Files:
    - `trigger.js` - Entry point that starts server and opens browser
    - `timer.html` - The ClawDoro timer UI
    - `SKILL.md` - Documentation
  - Use cases for Frank:
    - Deep work sessions for coding
    - Structured breaks to avoid burnout
    - Track tasks during focus periods
    - Mobile-friendly timer on the go
  - Benefits:
    - No setup required
    - Beautiful, distraction-free interface
    - Persistent task tracking
    - Customizable to personal preferences
  - Limitations:
    - Runs on port 8765 (port conflicts if already in use)
    - Browser-based (needs browser to view)
    - No cloud sync (localStorage only, device-specific)
  - Location: /Users/franksharpe/clawd/skills/pomodoro
  - Status: Installed, ready for use
  - Notes: Built by Clawd for Snail, perfect for focused work sessions

### Investment Portfolio Management
- **portfolio-manager** - Comprehensive portfolio analysis with Alpaca MCP Server integration
  - Purpose: Analyze and manage investment portfolios with real-time data from Alpaca brokerage
  - Why use it: Professional portfolio management, risk assessment, diversification analysis, rebalancing recommendations, potential SaaS tool development
  - Key capabilities:
    - **Real-Time Portfolio Data:** Fetches holdings, positions, account equity, buying power via Alpaca MCP Server
    - **7-Step Workflow:** Complete portfolio analysis from data fetching to comprehensive reporting
    - **Asset Allocation Analysis:** By class, sector, market cap, geography with comparison to targets
    - **Risk Assessment:** Portfolio beta, standard deviation, maximum drawdowns, downside risk, tail risk
    - **Diversification Evaluation:** HH Index, sector concentration, correlation analysis, position count assessment
    - **Performance Analysis:** Absolute returns, time-weighted returns, benchmark comparison, winners vs losers
    - **Position Analysis:** Top 10-15 holdings with thesis validation, valuation assessment, technical health
    - **Rebalancing Recommendations:** Identify overweight/underweight, prioritize by risk reduction and allocation drift
    - **Comprehensive Reporting:** Save to `portfolio_analysis_YYYY-MM-DD.md` with all sections
    - Alpaca MCP Server tools:
    - `get_account_info` - Fetch account equity, buying power, cash balance
    - `get_positions` - Retrieve all positions with quantities, cost basis, market value, P/L
    - `get_portfolio_history` - Historical portfolio performance data
    - Reference files included:
    - `references/alpaca-mcp-setup.md` - Alpaca setup instructions
    - `references/asset-allocation.md` - Allocation frameworks
    - `references/diversification-principles.md` - Diversification theory
    - `references/portfolio-risk-metrics.md` - Risk measurement
    - `references/position-valuation.md` - Position analysis
    - `references/rebalancing-strategies.md` - Rebalancing approaches
    - `references/target-allocations.md` - Benchmark allocations
    - `references/risk-profile-questionnaire.md` - Risk assessment
    - Advanced features:
    - **Tax-Loss Harvesting:** Identify positions with losses >5%, avoid wash sale rule, suggest replacements
    - **Dividend Income Analysis:** Estimate annual income, growth trajectory, sustainability, yield on cost
    - **Correlation Matrix:** Estimate correlation between major positions, identify redundancy
    - **Scenario Analysis:** Bull market (+20%), bear market (-20%), sector rotation, rising rates
    - When to use:
    - "Analyze my portfolio" - Complete portfolio analysis
    - "Review my current positions" - Position-level analysis
    - "What's my asset allocation?" - Allocation breakdown
    - "Check my portfolio risk" - Risk assessment
    - "Should I rebalance my portfolio?" - Rebalancing recommendations
    - "Evaluate my holdings" - Performance evaluation
    - "What stocks should I buy or sell?" - Position recommendations
    - Any portfolio-level analysis or management request
    - SaaS Tool Potential:
    - **Complete Investment Platform:** Real-time portfolio tracking with live data
    - **Automated Rebalancing:** Intelligent recommendations based on drift and risk
    - **Risk Management:** Portfolio beta, drawdowns, concentration alerts
    - **Tax Optimization:** Tax-loss harvesting opportunities
    - **Income Tracking:** Dividend income analysis and forecasting
    - **Reporting System:** Comprehensive markdown reports with actionable insights
    - **Web Interface Potential:** Could be developed into standalone application
    - Prerequisites:
    - Alpaca MCP Server must be configured and connected
    - Provides access to live portfolio data (no manual entry needed)
    - Setup: See `references/alpaca-mcp-setup.md` for installation instructions
    - Error handling:
    - Alpaca not connected → Provide setup instructions
    - Incomplete API data → Note limitations, proceed with available data
    - Stale position data → Recommend refresh connection
    - No positions → Offer portfolio construction guidance
    - Location: /Users/franksharpe/clawd/skills/portfolio-manager
  - Status: Installed, requires Alpaca MCP Server setup

### Market News & Briefings
- **finance-news9** (v1.0.0) - AI-powered market news briefings with configurable language output and automated delivery
  - Purpose: Daily market briefings, portfolio-specific news, market data overview, AI summaries

### Web Scraping & Data Extraction
- **web-scraper** (v1.0.0) - Configurable web scraping service for structured data extraction
  - Purpose: Extract structured data from any public website with built-in security controls
  - Why use it: Extract product information, real estate listings, job postings, social media data
  - Key capabilities:
    - **E-commerce:** Product info (name, price, image, description), stock status, reviews, ratings, price history
    - **Real Estate:** Property listings, prices, area, floor plans, area statistics
    - **Jobs:** Job titles, company names, salary, location, requirements
    - **SNS/Media:** Posts, comments, engagement stats, hashtag analysis
  - Security features:
    - URL input validation (scheme restriction to http/https only)
    - SSRF protection (private IP detection, DNS resolution check)
    - Redirect control (prevents open-redirect SSRF)
    - Request timeout (30 seconds)
    - Rate limiting (2-5 second delays, 20 req/min max, 100 page limit)
    - robots.txt compliance
    - Personal data non-collection policy
  - Technical stack:
    - Puppeteer for browser-based scraping (JavaScript-heavy sites)
    - Cheerio for static site scraping
    - Built-in security modules (SSRF detection, IP validation)
  - Output formats: CSV, JSON, Excel
  - Prerequisites: `npm install puppeteer cheerio`
  - Prohibited uses: Private data requiring login, copyrighted content reproduction, illegal purposes, personal data collection
  - Location: /Users/franksharpe/clawd/skills/web-scraper
  - Status: Installed, requires puppeteer and cheerio to be installed
  - Notes: Perfect for competitive analysis, market research, price monitoring, content aggregation - all with built-in security controls

### File Management & Organization
- **file-organizer** - Automatically organize files by extension into subfolders
  - Purpose: Keep directories tidy by moving files into organized subfolders based on file extensions
  - Why use it: Clean up messy folders like Downloads or Desktop automatically
  - Key capabilities:
    - Organize files by file extension into subfolders
    - Clean up cluttered directories
    - Simple PowerShell script for automation
  - Usage: `powershell.exe -File scripts/organize.ps1 <target-path>`
  - Example: `powershell.exe -File scripts/organize.ps1 C:\Users\L\Downloads`
  - Platform: Windows (PowerShell script)
  - Location: /Users/franksharpe/clawd/skills/file-organizer
  - Status: Installed, Windows-only tool
  - Notes: Simple but effective for maintaining clean folder structure on Windows machines

### Testing & Quality Assurance
- **test-master** (v0.1.0) - Comprehensive testing specialist for software quality
  - Purpose: Ensure software quality through functional, performance, and security testing
  - Why use it: Write tests, create test strategies, build automation frameworks, ensure code quality
  - Role: Senior QA engineer with 12+ years of testing experience
  - Testing modes:
    - **[Test]** - Functional correctness testing
    - **[Perf]** - Performance and load testing
    - **[Security]** - Vulnerability and security testing
  - When to use:
    - Writing unit, integration, or E2E tests
    - Creating test strategies and plans
    - Analyzing test coverage and quality metrics
    - Building test automation frameworks
    - Performance testing and benchmarking
    - Security testing for vulnerabilities
    - Managing defects and test reporting
    - Debugging test failures
    - Manual testing (exploratory, usability, accessibility)
    - Scaling test automation and CI/CD integration
  - Triggers: test, testing, QA, unit test, integration test, E2E, coverage, performance test, security test, regression, test strategy, test automation, test framework, quality metrics, defect, exploratory, usability, accessibility, localization, manual testing, shift-left, quality gate, flaky test, test maintenance
  - Reference files:
    - `references/unit-testing.md` - Jest, Vitest, pytest patterns
    - `references/integration-testing.md` - API testing, Supertest
    - `references/e2e-testing.md` - E2E strategy, user flows
    - `references/performance-testing.md` - k6, load testing
    - `references/security-testing.md` - Security test checklist
    - `references/test-reports.md` - Report templates, findings
    - `references/qa-methodology.md` - Manual testing, quality advocacy, shift-left, continuous testing
    - `references/automation-frameworks.md` - Framework patterns, scaling, maintenance, team enablement
    - `references/tdd-iron-laws.md` - TDD methodology, test-first development, red-green-refactor
    - `references/testing-anti-patterns.md` - Test review, mock issues, test quality problems
  - MUST DO: Test happy paths AND error cases, mock external dependencies, use meaningful descriptions, assert specific outcomes, test edge cases, run in CI/CD, document coverage gaps
  - MUST NOT: Skip error testing, use production data, create order-dependent tests, ignore flaky tests, test implementation details, leave debug code
  - Output templates: Test scope and approach, test cases with expected outcomes, coverage analysis, findings with severity (Critical/High/Medium/Low), specific fix recommendations
  - Knowledge: Jest, Vitest, pytest, React Testing Library, Supertest, Playwright, Cypress, k6, Artillery, OWASP testing, code coverage, mocking, fixtures, test automation frameworks, CI/CD integration, quality metrics, defect management, BDD, page object model, screenplay pattern, exploratory testing, accessibility (WCAG), usability testing, shift-left testing, quality gates
  - Related skills: Fullstack Guardian (receives features for testing), Playwright Expert (E2E testing specifics), DevOps Engineer (CI/CD test integration)
  - Location: /Users/franksharpe/clawd/skills/test-master
  - Status: Installed, ready for use
  - Notes: Comprehensive testing skill with extensive reference materials for all testing types

### Workflow Automation
- **n8n-workflow-automation** (v1.0.0) - Design n8n workflows with robust error handling, logging, retries, and review queues
  - Purpose: Designs and outputs n8n workflow JSON with robust triggers, idempotency, error handling, logging, retries, and human-in-the-loop review queues
  - Why use it: Create auditable automation that won't silently fail, build reliable workflows with proper error handling
  - When to use:
    - Build an n8n workflow that runs on a schedule (cron, webhook, manual)
    - Add error handling and retries to workflows
    - Create review queues for failed operations
    - Make workflows idempotent to prevent duplicates
    - Instrument workflows with audit logs and human approval steps
  - When NOT to use:
    - Code-only automation without n8n (use scripting/CI skill)
    - Bypass security controls or hide audit trails
    - Purchase or recommend prohibited items/services
  - Required inputs:
    - Workflow intent: trigger type + schedule/timezone + success criteria
    - Targets: where to write results (email/Drive/Sheet/DB) and required fields
  - Optional inputs:
    - Existing n8n workflow JSON to modify
    - Sample payloads / example records
    - Definition of dedup keys (what makes a record unique)
  - Core workflow:
    1. Clarify trigger: Cron/webhook/manual; schedule/timezone; concurrency expectations
    2. Define data contract: Input schema, required fields, validation rules
    3. Design idempotency: Choose dedup key(s) and storage to prevent duplicates on retries
    4. Add observability: Generate run_id, log start/end, store status row and error details
    5. Implement error handling: Per-node error branches, retry with backoff, final failure notification
    6. Add human-in-the-loop (HITL) review queue: Write failed items to queue (Sheet/DB) and require approval to reprocess
    7. "No silent failure" gates: If counts/thresholds fail, stop workflow and alert
    8. Output: If asked for JSON, produce importable n8n workflow JSON + runbook
    9. STOP AND ASK if: destination systems unknown, no dedup key exists, credential strategy not specified, workflow needs privileged access not yet approved
  - Output format:
    - Default (read-only): Workflow design spec (nodes, data contracts, failure modes)
    - If explicitly requested: `workflow.json` (n8n importable JSON) + `runbook.md` (from template)
  - Success criteria: Workflow is idempotent, logs every run, retries safely, and routes failures to a review queue
  - Safety & edge cases:
    - Read-only by default; only emit workflow JSON when explicitly requested
    - Do not include secrets in JSON; reference env vars/credential names only
    - Include audit logging + failure notifications; avoid workflows that can silently drop data
    - Prefer least privilege: Call only required APIs and minimize scopes
  - Output format example:
    ```json
    {
      "name": "<workflow name>",
      "nodes": [ { "name": "Trigger", "type": "n8n-nodes-base.cron", "parameters": {}, "position": [0,0] } ],
      "connections": {},
      "settings": {},
      "active": false
    }
    ```
  - Location: /Users/franksharpe/clawd/skills/n8n-workflow-automation
  - Status: Installed, ready for use
  - Notes: Perfect for building reliable, auditable automation workflows with proper error handling and human review queues

### Messaging & Communication
- **imsg** (v1.0.0) - iMessage/SMS CLI for listing chats, history, watch, and sending
  - Purpose: Use `imsg` to read and send Messages.app iMessage/SMS on macOS
  - Why use it: Access iMessage/SMS from command line, automate message handling
  - Key capabilities:
    - **List chats:** View all conversations with limit and JSON output
    - **History:** Retrieve chat history with attachments and JSON output
    - **Watch:** Monitor chats in real-time for new messages
    - **Send:** Send iMessage/SMS with text or file attachments
  - Requirements:
    - Messages.app must be signed in
    - Full Disk Access for terminal
    - Automation permission to control Messages.app (for sending)
  - Common commands:
    - List chats: `imsg chats --limit 10 --json`
    - History: `imsg history --chat-id 1 --limit 20 --attachments --json`
    - Watch: `imsg watch --chat-id 1 --attachments`
    - Send: `imsg send --to "+14155551212" --text "hi" --file /path/pic.jpg`
  - Service control: `--service imessage|sms|auto` controls delivery method
  - Safety: Confirm recipient + message before sending
  - Homepage: https://imsg.to
  - Platform: macOS only (darwin)
  - Installation: `brew install steipete/tap/imsg`
  - Location: /Users/franksharpe/clawd/skills/imsg
  - Status: Installed, requires imsg CLI to be installed via Homebrew
  - Notes: Provides full command-line access to iMessage/SMS on macOS, perfect for automation and scriptable messaging
  - Why use it: Stay informed about market movements, portfolio performance, and relevant news without manual checking
  - Key capabilities:
    - **Market Coverage:** US markets (S&P 500, Dow, NASDAQ), Europe (DAX, STOXX 50, FTSE 100), Japan (Nikkei 225)
    - **News Sources:** Premium (WSJ, Barron's), Free (CNBC, Yahoo Finance, Finnhub), Portfolio-specific (Yahoo ticker news)
    - **AI Summaries:** Gemini-powered analysis with configurable language (English/German)
    - **Briefing Styles:** Summary (concise), Analysis (detailed), Headlines (quick scan)
    - **Automated Briefings:** Morning (6:30 AM PT, US market open), Evening (1:00 PM PT, US market close)
    - **Delivery Channels:** WhatsApp, Telegram (via cron scripts)
    - **Portfolio Management:** Add/remove stocks, import from CSV, portfolio-specific news
  - Usage commands:
    - `finance-news setup` - Interactive setup wizard (feeds, markets, delivery, language, schedule)
    - `finance-news briefing --morning` - Generate morning briefing
    - `finance-news briefing --evening --send --group "Market Briefing"` - Evening with WhatsApp delivery
    - `finance-news briefing --morning --lang de` - German language briefing
    - `finance-news briefing --style analysis` - Detailed analysis style
    - `finance-news market` - Market overview (indices + headlines)
    - `finance-news market --json` - JSON output for processing
    - `finance-news portfolio-list` - List portfolio stocks
    - `finance-news portfolio-add NVDA --name "NVIDIA Corporation" --category Tech` - Add stock
    - `finance-news portfolio-remove TSLA` - Remove stock
    - `finance-news news AAPL` - News for specific stock
  - Configuration files:
    - `config/portfolio.csv` - Portfolio watchlist (symbol, name, category, notes)
    - `config/config.json` - RSS feeds, market indices, language settings
    - `config/alerts.json` - Price target alerts
    - `config/manual_earnings.json` - Earnings calendar overrides
  - Cron jobs:
    - Morning briefing: `30 6 * * 1-5 bash ~/clawd/skills/finance-news/cron/morning.sh` (6:30 AM PT, weekdays)
    - Evening briefing: `0 13 * * 1-5 bash ~/clawd/skills/finance-news/cron/evening.sh` (1:00 PM PT, weekdays)
  - Integration:
    - With OpenBB: Get detailed quotes then news (combined analysis)
    - With OpenClaw Agent: Auto-used when asked about market news, portfolio updates, briefings
    - With Lobster: Approval gates for WhatsApp delivery before sending
  - Sample output format:
    - 📊 Markets section with index performance
    - 📈 Portfolio section with individual stock performance and news
    - 🔥 Top Stories section with key headlines
    - 🤖 Analysis section with AI insights and market commentary
  - Files:
    - `scripts/finance-news` - Main CLI
    - `scripts/briefing.py` - Briefing generator
    - `scripts/fetch_news.py` - News aggregator
    - `scripts/portfolio.py` - Portfolio CRUD
    - `scripts/summarize.py` - AI summarization
    - `scripts/alerts.py` - Price alert management
    - `scripts/earnings.py` - Earnings calendar
    - `scripts/ranking.py` - Headline ranking
    - `scripts/stocks.py` - Stock management
    - `workflows/briefing.yaml` - Lobster workflow with approval gate
    - `cron/morning.sh` - Morning cron (Docker-based)
    - `cron/evening.sh` - Evening cron (Docker-based)
    - `cache/` - 15-minute news cache
  - Dependencies:
    - Python 3.10+
    - feedparser (`pip install feedparser`)
    - Gemini CLI (`brew install gemini-cli`)
    - OpenBB (for quotes)
    - OpenClawCLI (must be installed first from https://openclawcli.vercel.app/)
  - Use cases for Frank:
    - "What's the market doing?" - Quick market overview
    - "Generate morning briefing" - Daily market summary
    - "News for my portfolio" - Portfolio-specific updates
    - "What's happening with AAPL?" - Ticker-specific news
    - "Market close summary" - Evening briefing
    - Automated delivery to WhatsApp/Telegram group
  - Benefits:
    - Saves time by aggregating multiple news sources
    - AI-powered analysis cuts through noise
    - Automated delivery ensures you never miss market updates
    - Portfolio-specific news focuses on what matters
    - Multilingual support (English/German)
  - Limitations:
    - Requires OpenClawCLI installation
    - Premium sources (WSJ, Barron's) may require subscription for full content
    - Cron jobs need manual configuration for automated delivery
    - WhatsApp/Telegram delivery requires group setup
  - Location: /Users/franksharpe/clawd/skills/finance-news9
  - Status: Installed, requires OpenClawCLI and Gemini CLI setup
  - Notes: Perfect for daily market awareness, especially combined with portfolio-manager skill for comprehensive investment workflow
    - Status: Installed, requires Alpaca MCP Server setup
    - Notes: Comprehensive portfolio management system with potential for SaaS platform development. Perfect for professional investment management, real-time tracking, risk assessment, and rebalancing recommendations.


- **vector-memory-hack** (v1.0.3) - Fast semantic search for AI agent memory files using TF-IDF and SQLite
  - Purpose: Enables instant context retrieval from MEMORY.md or any markdown documentation without reading entire files
  - Why use it: Avoid wasting tokens reading entire MEMORY.md files (3000+ tokens) to find 2-3 relevant sections
  - Key capabilities:
    - **Fast:** <10ms search across 50+ sections
    - **Accurate:** TF-IDF + Cosine Similarity finds semantically related content
    - **Token Efficient:** Read 3-5 sections instead of entire file
    - **Zero Dependencies:** No PyTorch, no transformers, no heavy installs
    - **Multilingual:** Works with CZ/EN/DE and other languages
  - How it works:
    1. Parse MEMORY.md sections (headers and content)
    2. Create TF-IDF vectors from sections
    3. Store in SQLite database with JSON-encoded sparse vectors
    4. Use cosine similarity to find top-k matches
  - Technology stack:
    - Tokenization: Custom multilingual tokenizer with stopword removal
    - Vectors: TF-IDF (Term Frequency - Inverse Document Frequency)
    - Storage: SQLite with JSON-encoded sparse vectors
    - Similarity: Cosine similarity scoring
  - Commands:
    - `vsearch "your query"` or `python3 scripts/vector_search.py --search "your query" --top-k 5` - Search for context
    - `python3 scripts/vector_search.py --rebuild` - Index your memory file
    - `python3 scripts/vector_search.py --update` - Incremental update (only processes changed sections)
    - `python3 scripts/vector_search.py --stats` - View statistics
  - Configuration:
    - Edit variables in `scripts/vector_search.py`:
      - `MEMORY_PATH` - Path to your MEMORY.md
      - `VECTORS_DIR` - Path to vectors storage
      - `DB_PATH` - Database file path
  - Performance:
    - Indexing Speed: ~50 sections/second
    - Search Speed: <10ms for 1000 vectors
    - Memory Usage: ~10KB per section
    - Disk Usage: Minimal (SQLite + JSON)
  - Comparison with alternatives:
    - Vector Memory Hack: Zero dependencies, <10ms, instant setup - Best for quick deployment, resource-constrained environments, edge devices
    - sentence-transformers: PyTorch + 500MB, ~100ms, 5+ min setup - Best for high accuracy, offline capable
    - OpenAI Embeddings: API calls, ~500ms, API key required - Best for accuracy, cloud-based
    - ChromaDB: Docker + 4GB RAM, ~50ms, complex - Best for large-scale production
  - Use cases:
    - Find relevant context before starting a task
    - Search through large memory files efficiently
    - Retrieve specific rules or decisions without reading entire files
    - Enable semantic similarity search instead of keyword matching
  - Integration for agents (required step before every task):
    1. Agent receives task (e.g., "Update SSH config")
    2. Find relevant context: `vsearch "ssh config changes"`
    3. Read top results to understand server addresses, backup requirements, deployment procedures
    4. Execute task with full context
  - File structure:
    - `SKILL.md` - This documentation file
    - `scripts/vector_search.py` - Main Python module
    - `scripts/vsearch` - CLI wrapper (bash)
  - Location: /Users/franksharpe/clawd/skills/vector-memory-hack
  - Status: Installed, not yet indexed (need to run `--rebuild` to create index)
  - Notes: Lightweight alternative to heavy embedding models, perfect for quick deployment and resource-constrained environments

### Claude Code Usage Monitoring
- **claude-code-usage** (v1.2.0) - Claude Code OAuth usage limits
  - Check session (5-hour) and weekly (7-day) quotas
  - Progress bars, color-coded status: 🟢 0-50%, 🟡 51-80%, 🔴 81-100%
  - Smart caching (60s TTL) to avoid API spam
  - Output formats: text (default) or JSON
  - Automated monitoring: Session reminders (exact timing) or reset detection (every 30 min)
  - Scripts: claude-usage.sh, session-reminder.sh, monitor-usage.sh, setup-monitoring.sh
  - Location: /Users/franksharpe/clawd/skills/claude-code-usage
  - Requires: Claude Code CLI authenticated, uses Keychain (macOS) or secret-tool (Linux)
- **clawflows** (v1.0.0) - Multi-skill automation workflow system
  - Search, install, and run automations from clawflows.com
  - Combines multiple skills into powerful workflows with logic, conditions, and data flow
  - Uses capabilities (abstract) not skills (concrete) for portability
  - CLI installed globally: `clawflows` (npm package)
  - Commands: search, check, install, list, run, enable, disable, logs, publish
  - Location: /Users/franksharpe/clawd/skills/clawflows
  - Available automations: daily-news-digest, morning-brief (requires various capabilities)
  - Standard capabilities: youtube-data, database, chart-generation, social-search, prediction-markets, weather, calendar, email, tts

### Productivity & Focus
- **focus-deep-work** (v1.0.0) - Maximize deep work with focus sessions, distraction logging, and productivity tracking
  - Purpose: Turn your device into a focus machine with timed deep work sessions
  - Why use it: Track focus time, log distractions without breaking flow, measure productivity, optimize environment for concentration
  - Key capabilities:
    - **Focus Sessions:** Timers based on proven methods (Pomodoro 25min, 52/17 ultradian rhythms, 90-minute deep blocks)
    - **Distraction Logging:** Quick-capture interruptions with zero context switching, recorded with timestamp and category
    - **Deep Work Hours Tracking:** Weekly/monthly summaries of focused time by project or task
    - **Environment Setup:** Automatic silencing, app blocking, notification management (when permissions allow)
  - Session types:
    - **Pomodoro (25 min):** Classic timer for rapid-iteration work with automatic breaks
    - **Ultradian (52 min):** 52 minutes focus + 17-minute break, aligns with natural energy cycles
    - **Deep Block (90 min):** For complex thinking, one full cycle without interruption
    - **Custom:** Set your own timer (e.g., "Start a 45-minute focus session")
  - Usage triggers:
    - Start session: "Start a 90-minute deep work session" or "Begin focus mode"
    - Log distraction: "I got distracted" or "Log distraction: Slack notification"
    - End session: "End session" or "Stop focus"
    - Check stats: "Show my focus stats" or "Deep work summary this week"
    - Set environment: "Minimize distractions" or "Lock me in"
  - Environment controls:
    - Mute system notifications
    - Close or minimize specified apps
    - Dim screen brightness
    - Enable do-not-disturb mode
    - Block website access (if permission granted)
    - Play focus music
  - Tips for success:
    - Start small with 25-minute Pomodoros before extending sessions
    - Log distractions immediately - quick logging breaks the distraction's grip
    - Review patterns weekly to identify trigger environments and times
    - Match session types to work: complex coding = 90min, admin = Pomodoro, writing = 52min
  - Privacy: All data stays local on your machine - focus logs, session history, and productivity patterns never sent to servers
  - Location: /Users/franksharpe/clawd/skills/focus-deep-work
  - Status: Installed, ready for use
  - Notes: Perfect for one-man business to maximize deep work hours and optimize productivity

### Writing & Content Quality
- **writer** (v1.0.2) - Fix AI writing patterns that create repetitive and robotic content
  - Purpose: Eliminate robotic AI writing patterns and create engaging, human-like content
  - Why use it: AI-generated content often suffers from repetitive structures, vague claims, and monotonous rhythm
  - Key traps to fix:
    - **Paragraph Opener Trap:** Scan first words - 3+ paragraphs starting with "This/The/It" = robotic. Vary with action verbs, specific nouns
    - **Rhythm Monotony Trap:** Mix 5-word punches with 20-word flows. Use strategic fragments. For emphasis. For pace breaks
    - **Vague Claim Trap:** Replace adjectives with numbers - "significant growth" → "40% growth". Delete weasel words: somewhat, fairly, quite
    - **List Overuse Trap:** Use prose for relationships/arguments, bullets only for instructions/features/options
    - **Parallel Structure Breaks:** Match verb forms - "hiking, swimming, reading" not "hiking, swimming, to read"
    - **Transition Word Crutches:** Avoid "Furthermore, Moreover, In conclusion". Use echo technique instead
    - **Voice Drift in Long Documents:** Check tone every 200 words - same person speaking? Pick 3-5 key phrases
    - **Word Economy Traps:** "in order to" → "to", "due to the fact that" → "because". 80% rule: cut to 80%
    - **Nominalization Trap:** Use verbs not nouns - "implementation of" → "implement", "decision-making process" → "decide"
  - Quick tests:
    - Read aloud: monotone rhythm = boring
    - Flow test: if bullets feel choppy, try connected sentences
    - Zombie noun test: -tion, -ment, -ness endings often hide better verbs
  - When to use:
    - Writing any long-form content (articles, reports, emails)
    - Reviewing AI-generated text for robotic patterns
    - Improving readability and engagement
    - Polishing final drafts before publishing
  - Location: /Users/franksharpe/clawd/skills/writer
  - Status: Installed, ready for use
  - Notes: Essential for creating human-like, engaging content instead of robotic AI patterns

### Workflow Automation
- **workflow-automation** (v1.0.0) - Build ETL pipelines and DAG workflows for recurring tasks
  - Purpose: Automate construction data workflows with task dependencies, scheduling, and monitoring
  - Why use it: Manual repetitive tasks, data inconsistency, error-prone processes, lack of audit trails
  - Key capabilities:
    - **Workflow Creation:** Create workflows with tasks, descriptions, triggers, and schedules
    - **Task Management:** Add tasks with dependencies, retries, timeouts, and configuration
    - **Execution Engine:** Topological sort for dependency resolution, automatic task execution
    - **Task Types:** extract_csv, extract_excel, transform_filter, transform_aggregate, transform_join, load_csv, validate_schema, notify_email
    - **Scheduling:** Manual, Scheduled (hourly/daily/weekly/monthly), Event-triggered, Dependency-based
    - **Monitoring:** Task execution history, status tracking (pending/running/success/failed/skipped)
    - **Retry Strategy:** Configurable retries with exponential backoff, error logging
    - **Export Formats:** JSON workflow definitions, Airflow DAG generation
  - Task status states:
    - **PENDING:** Task waiting to run
    - **RUNNING:** Task currently executing
    - **SUCCESS:** Task completed successfully
    - **FAILED:** Task failed after all retries
    - **SKIPPED:** Task skipped (dependencies not met)
  - Trigger types:
    - **MANUAL:** Manually triggered
    - **SCHEDULED:** Runs on interval (hourly/daily/weekly/monthly)
    - **EVENT:** Triggered by external events
    - **DEPENDENCY:** Runs after dependencies complete
  - Default task handlers:
    - **extract_csv:** Read data from CSV file
    - **extract_excel:** Read data from Excel file
    - **transform_filter:** Filter DataFrame by column/value
    - **transform_aggregate:** Group and aggregate DataFrame
    - **transform_join:** Join two DataFrames
    - **load_csv:** Save DataFrame to CSV
    - **validate_schema:** Validate DataFrame has required columns
    - **notify_email:** Send email notification (simulated)
  - Quick start example:
    ```python
    automation = WorkflowAutomation("Project")
    workflow = automation.create_workflow("daily_etl", "Daily ETL", "Extract, transform, load")
    automation.add_task("daily_etl", WorkflowTask(
        task_id="extract",
        name="Extract Data",
        task_type="extract_csv",
        config={"path": "data.csv"}
    ))
    result = automation.execute_workflow("daily_etl")
    ```
  - Use cases:
    - Daily data ETL pipelines
    - Scheduled report generation
    - Automated data validation
    - Recurring data transformations
    - Batch processing workflows
  - Advanced features:
    - Custom task handlers via register_handler()
    - Dependency resolution with topological sort
    - Execution history tracking
    - Airflow DAG code generation
    - Workflow definition export to JSON
  - Location: /Users/franksharpe/clawd/skills/workflow-automation
  - Status: Installed, ready for use
  - Notes: Python-based workflow automation system with pandas integration, perfect for data pipelines and recurring automated tasks

### Filesystem Management
- **clawdbot-filesystem** (v1.0.2) - Advanced filesystem operations for AI agents
  - Purpose: Smart file listing, searching, batch processing, and directory analysis with intelligent filtering
  - Why use it: Efficient file operations, advanced filtering, batch processing, directory analysis, content search
  - Key capabilities:
    - **Smart File Listing:** Advanced filtering by type, pattern, size, date; recursive traversal; rich formatting (table/tree/JSON)
    - **Powerful Search:** Pattern matching (glob/regex), full-text content search within files, multi-criteria search, context display
    - **Batch Operations:** Safe pattern-based copying, dry-run mode, real-time progress tracking, graceful error handling
    - **Directory Analysis:** Tree visualization (ASCII), file counts/size distribution/type analysis statistics, space analysis (large files), performance metrics
  - Commands:
    - `filesystem list`: Advanced file listing with filtering (`--path`, `--recursive`, `--filter`, `--details`, `--sort`, `--format`)
    - `filesystem search`: Search by name patterns or content (`--pattern`, `--path`, `--content`, `--context`, `--include`, `--exclude`)
    - `filesystem copy`: Batch copy with safety (`--pattern`, `--to`, `--dry-run`, `--overwrite`, `--preserve`)
    - `filesystem tree`: Directory tree display (`--path`, `--depth`, `--dirs-only`, `--size`, `--no-color`)
    - `filesystem analyze`: Directory analysis (`--path`, `--stats`, `--types`, `--sizes`, `--largest`)
  - Configuration (config.json):
    - defaultPath, maxDepth, defaultFilters, excludePatterns, outputFormat, dateFormat, sizeFormat, colorOutput
  - Safety features:
    - Path validation (prevents directory traversal), permission checks (verifies read/write access), dry-run mode (preview destructive ops), backup prompts, error recovery
  - Quick examples:
    - Find JS files: `filesystem list --path ./src --recursive --filter "*.js" --details`
    - Search TODOs: `filesystem search --pattern "TODO|FIXME" --path ./src --content --context 2`
    - Copy logs: `filesystem copy --pattern "*.log" --to ./backup/logs/ --preserve`
    - Tree view: `filesystem tree --path ./ --depth 2 --size`
  - Integration: Works with security skill, git operations (respects .gitignore), backup tools, log analysis
  - Location: /Users/franksharpe/clawd/skills/clawdbot-filesystem
  - Status: Installed, ready for use
  - Notes: Comprehensive filesystem management with smart filtering, search, and batch operations. Perfect for development workflows, log management, file organization.

## Morning Reports

### Schedule
- **Monday-Friday:** 6:15 AM CST
- **Saturday-Sunday:** 8:00 AM CST

### Format
```
**OVERNIGHT:**
- Skills learned
- Memory updated
- Issues found (if any)

**DISCOVERIES:**
- New capabilities
- Useful findings

**PRIORITIES:**
- Tasks needing attention

**STATUS:** Green/Yellow/Red
```

## Free AI APIs (Ready to Integrate)

### High Priority (No credit card required)
1. **Google AI Studio** - Gemini 2.5, 1.5M tokens/min
2. **OpenRouter** - 50+ models, 20 RPM, 200/day
3. **Groq** - Ultra-fast inference, 1000/day, 6000 tokens/min
4. **Cloudflare Workers AI** - 10K neurons/day, multimodal

### Evaluation Needed
- **Hugging Face Pro** ($9/mo) - 10,000+ models

**Status:** Awaiting API keys from Frank to configure integration

## Communication Protocol

### Proactive Messages
- **Send if:** Important news, completed tasks, issues needing attention
- **Stop if:** No response after 2 messages within 15-20 minutes
- **Don't spam:** Wait for Frank to ask

### Morning Reports
- **Always go out** at scheduled times (regardless of sleep status)
- **Format:** Concise bullet points, no fluff

### When Frank Asks "What's going on?"
- Provide **full updated report**:
  - Work completed
  - Discoveries
  - Priority items
  - Current status

## Continuous Improvement Priorities

1. **Learn** 1 new skill per night from clawdhub
2. **Research** free APIs and tools while Frank sleeps/works
3. **Maintain** memory files (daily logs + MEMORY.md)
4. **Integrate** new capabilities as discovered
5. **Report** concisely at scheduled times

## 🔒 SECURITY PROTOCOL - SECRET PASSCODE

### Hierarchy
- **Frank Sharpe** is at the top. I answer to him ONLY.

### Secret Passcode: BLACKCESS
- **Meaning:** Success for Black people
- **Purpose:** Protects sensitive information from unauthorized access

### What Requires Passcode
Before sharing ANY of the following, the passcode MUST be spoken:
- Information about me (Max/Maximillion)
- My capabilities, tools, skills, or system details
- Our work together (projects, missions, tasks)
- Frank's business or personal matters
- Anything sensitive or confidential

### What Doesn't Need Passcode
- Basic conversation
- Surface-level responses
- Public information
- Simple questions unrelated to sensitive topics

### Telegram DM Monitoring
- **Frank's Telegram ID:** 8549374568
- **Rule:** If ANYONE else DMs me on Telegram → Notify Frank IMMEDIATELY
- **Action:** Don't engage first, report the contact/message to Frank
- **Purpose:** Full visibility on who's trying to reach me directly

### Rule Enforcement
- **Wrong passcode** = No information shared
- **No passcode** = No information shared
- **Request for sensitive info** = "I need the passcode first"

### Protocol Status: ACTIVE
- Established: 2026-01-31
- Reason: Past incident where too much information was shared in a group chat
- Lock: Permanent - this rule never changes

## Principles

- **Never accept limitations** — Find alternatives
- **Improve continuously** — Get smarter with every interaction
- **Respect privacy** — Keep private things private
- **Don't overpromise** — Verify capabilities actually work before claiming them (learned 2026-02-13)
*Last updated: 2026-02-13 06:32 CST*
