# SOMA Studio Token Optimization Guide

## SESSION INITIALIZATION RULE (Copy to System Prompt)

On every session start:
1. Load ONLY these files:
   - SOUL.md
   - USER.md
   - IDENTITY.md
   - memory/YYYY-MM-DD.md (if it exists)

2. DO NOT auto-load:
   - MEMORY.md
   - Session history
   - Prior messages
   - Previous tool outputs

3. When user asks about prior context:
   - Use memory_search() on demand
   - Pull only the relevant snippet with memory_get()
   - Don't load the whole file

4. Update memory/YYYY-MM-DD.md at end of session with:
   - What you worked on
   - Decisions made
   - Leads generated
   - Blockers
   - Next steps

**Result:** 80% context overhead reduction (50KB → 8KB)

---

## MODEL ROUTING RULE (Add to System Prompt)

**Default:** Always use Haiku (or free tier equivalent)
**Switch to Sonnet ONLY when:**
- Architecture decisions
- Production code review
- Security analysis
- Complex debugging/reasoning
- Strategic multi-project decisions

**Result:** 90% token cost reduction

---

## RATE LIMITS (Add to System Prompt)

- 5 seconds minimum between API calls
- 10 seconds between web searches
- Max 5 searches per batch, then 2-minute break
- Batch similar work (one request for 10 items, not 10 requests)
- If you hit 429 error: STOP, wait 5 minutes, retry

**Result:** Prevent runaway automation costs

---

## IMPLEMENTATION STATUS

✅ Session Initialization: READY
✅ Model Routing: READY  
✅ Rate Limits: READY
🔄 Heartbeat to Ollama: PENDING
🔄 Prompt Caching: PENDING