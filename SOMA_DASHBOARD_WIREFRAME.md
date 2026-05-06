# SOMA Studio Dashboard Wireframe
## Real-Time Agent Tycoon Interface

## 🎮 **Dashboard Layout**

```
┌─────────────────────────────────────────────────────────────┐
│  SOMA STUDIO - AGENT TYCOON v1.0                           │
├─────────────────────────────────────────────────────────────┤
│  💰 REVENUE: $0.00/mo     📈 GROWTH: 0%     🚀 STATUS: ON  │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  ┌──────────────┐ ┌──────────────┐ ┌──────────────┐        │
│  │   BEACON     │ │    HELM      │ │    VERSE     │        │
│  │  📊 RESEARCH │ │  🎯 DIRECTION│ │  ✍️ WRITING  │        │
│  │  STATUS: ✅   │ │  STATUS: ⏳   │ │  STATUS: ❌   │        │
│  │  TOPICS: 0   │ │  APPROVED: 0 │ │  SCRIPTS: 0  │        │
│  └──────────────┘ └──────────────┘ └──────────────┘        │
│                                                             │
│  ┌──────────────┐ ┌──────────────┐ ┌──────────────┐        │
│  │   CHORUS     │ │    BLADE     │ │   FRAME      │        │
│  │  🗣️ VOICE    │ │  ✂️ EDITING  │ │  🎨 THUMB    │        │
│  │  STATUS: ❌   │ │  STATUS: ❌   │ │  STATUS: ❌   │        │
│  │  PROMPTS: 0  │ │  EDL: 0      │ │  CONCEPTS: 0 │        │
│  └──────────────┘ └──────────────┘ └──────────────┘        │
│                                                             │
├─────────────────────────────────────────────────────────────┤
│  📋 CURRENT PIPELINE                                          │
│  ┌─────────────────────────────────────────────────────────┐│
│  │ #1: [WAITING] Research Phase                           ││
│  │ #2: [WAITING] Script Writing                           ││
│  │ #3: [WAITING] Voice Production                         ││
│  │ #4: [WAITING] Video Editing                            ││
│  └─────────────────────────────────────────────────────────┘│
│                                                             │
├─────────────────────────────────────────────────────────────┤
│  📊 PERFORMANCE METRICS                                     │
│  Views: 0 | Subscribers: 0 | CTR: 0% | Retention: 0%        │
└─────────────────────────────────────────────────────────────┘
```

## 🎯 **Agent Status Indicators**

### Colors
- **✅ Active/Green** - Agent working
- **⏳ Waiting/Yellow** - Blocked or queued
- **❌ Idle/Red** - Not active
- **💥 Error/Orange** - Something broke

### Status Popups
Click any agent to see:
- Current task
- Progress bar
- Last update
- Output preview

## 🎬 **Production Pipeline Tracker**

### Long-form Pipeline
1. **BEACON** → Research complete
2. **HELM** → Direction approved
3. **VERSE** → Script written
4. **CHORUS** → VO prompts ready
5. **BLADE** → EDL generated
6. **FRAME** → Thumbnail concept

### Shorts Pipeline
1. **BEACON** → Trending topics
2. **VERSE** → Hook + beats
3. **CHORUS** → VO direction
4. **BLADE** → Pacing cut
5. **FRAME** → Caption graphics

## 📊 **Real-Time Metrics Panel**

### Revenue Tracking
- **Current:** $0.00/month
- **Projected:** $0.00/month
- **Goal:** $10,000/month

### Performance
- **Views:** 0
- **Subscribers:** 0
- **CTR:** 0%
- **Retention:** 0%

### Production Stats
- **Videos Today:** 0
- **Shorts Queue:** 0
- **Long-form Queue:** 0
- **Published This Week:** 0

## 🔧 **CLI Integration**

### Dashboard Commands
```bash
# Start pipeline
/yt-pulse

# Script only
/yt-script

# Shorts only
/shorts-script

# Thumbnail only
/thumbnail

# Check status
/dashboard-status
```

### API Endpoints
```
GET /api/agents/status
GET /api/pipeline/current
GET /api/metrics/performance
GET /api/videos/queue
POST /api/trigger/pipeline
```

## 🎨 **Visual Design**

### Color Scheme
- **Primary:** #1A1A1A (Charcoal)
- **Accent:** #B8860B (Ember)
- **Text:** #F5F5DC (Cream)
- **UI:** #2A2A2A (Dark gray)

### Typography
- **Headers:** Fraunces (serif)
- **Body:** Inter (sans-serif)
- **Captions:** League Spartan (bold)

### Animations
- **Status changes:** Smooth transitions
- **Progress bars:** Real-time fill
- **Agent movement:** Game-like physics

## 🚀 **Implementation Roadmap**

### Phase 1: Core Dashboard
- [ ] Basic layout
- [ ] Agent status display
- [ ] Pipeline tracker
- [ ] Metrics panel

### Phase 2: Real-Time Updates
- [ ] WebSocket integration
- [ ] Live status changes
- [ ] Progress animations
- [ ] Sound effects

### Phase 3: Advanced Features
- [ ] Click-to-expand agents
- [ ] Performance graphs
- [ ] Revenue projections
- [ ] Export data

## 📁 **File Structure**

```
~/Claude/quiet-revolution-studio/
├── dashboard/
│   ├── index.html
│   ├── style.css
│   ├── script.js
│   └── api/
├── agents/
│   ├── beacon.js
│   ├── helm.js
│   ├── verse.js
│   ├── chorus.js
│   ├── blade.js
│   └── frame.js
└── pipeline/
    ├── shorts/
    ├── longform/
    └── thumbnails/
```

## 🎯 **Next Actions**

1. **Build Dashboard** - HTML/CSS/JS
2. **Connect Agents** - WebSocket API
3. **Test Pipeline** - End-to-end flow
4. **Deploy Live** - Real-time interface

**The dashboard will show your agents working like a video game!** 🎮