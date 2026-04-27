# PRD: Hidden Gems — Curated Restaurant Discovery on Swiggy Dineout

## 1. Problem Statement

Users browsing Swiggy Dineout repeatedly see the same 50-75 highly-rated restaurants, limiting discovery to "obvious" choices. Meanwhile, 200-300 equally high-quality restaurants (4.0+ rating) go undiscovered due to low review volume, missing out on customer visits and revenue. This creates a **discovery fatigue problem for users** and an **invisible inventory problem for Swiggy** — the platform isn't leveraging its full high-quality restaurant base for engagement and GMV.

---

## 2. Background & Context

### Why This Matters Now

**Market Context:**
- Dine-out discovery is dominated by Zomato's algorithmic sorting (popularity bias)
- Fine dine platforms (EazyDiner, MakeMyTrip Travel) position themselves as "curated experiences"
- Users crave authentic, non-obvious recommendations (vs algorithm fatigue)

**Internal Data (EDA Finding):**
- Zomato Bangalore has 200-300 "hidden gems" — restaurants with 4.0+ rating but <200 votes
- These hidden gems have **identical quality** as highly-voted restaurants (both ~4.2 avg rating)
- But they get **5-10x lower visibility** (e.g., 50 votes vs 500 votes)
- These high-quality, low-visibility restaurants are distributed across ALL locations, including underserved areas

**Swiggy Dineout Opportunity:**
- Differentiate from Zomato by curating (human + data) instead of sorting (algorithm only)
- Expand addressable inventory — tap the 200+ undiscovered gems
- Build user habit through "discovery" engagement (weekly gem updates)
- Drive reservation volume for Swiggy's restaurant partners (especially tier-2 restaurants)

---

## 3. Target User

### Persona 1: Weekend Casual Diner 🎯
**Name:** Priya, 26, Software Engineer  
**Goals:**
- Find a nice restaurant for Friday evening with friends
- Discover something NEW each time (tired of same restaurants)
- Want good quality without being too fancy or expensive

**Frustrations:**
- Zomato always shows same 30 restaurants in Koramangala
- Doesn't trust "new" restaurants (no reviews = risky)
- Can't differentiate between casual and fine dine easily

**Behavior:**
- Browses Swiggy Dineout on Friday evening
- Filters by location + cuisine
- Reads top 5 restaurants' reviews
- Books same 3 restaurants repeatedly (predictable)

**Why Hidden Gems Matters:**
- Surfaced gems have >4.0 rating (low risk, same as familiar restaurants)
- Gem badge = social proof ("others rated it high, it's just undiscovered")
- Variety = weekly new options to try

---

### Persona 2: Food Explorer 🎯
**Name:** Akshay, 28, Marketing Manager  
**Goals:**
- Discover hidden, authentic restaurants (not tourist traps)
- Try different cuisines, occasions (date nights, business dinners, casual hangouts)
- Be first among friends to discover new places

**Frustrations:**
- Zomato recommendations are obvious (high votes = mainstream)
- Fine dine platforms (EazyDiner) have limited inventory in Bangalore
- Can't filter by quality + occasion easily

**Behavior:**
- Actively searches for "new openings," "food explorers," "undiscovered gems"
- Follows food bloggers for recommendations
- Willing to try 4.0-rated restaurant with 50 votes (trusts quality over popularity)
- Shares discoveries on Instagram/LinkedIn

**Why Hidden Gems Matters:**
- Exclusive discovery feature (not everyone sees these gems)
- Personalization by occasion (fine dine gems vs casual gems)
- Build brand loyalty (Swiggy Dineout = place to discover first)

---

## 4. Goals & Success Metrics

### User Goals
1. **Discover high-quality restaurants I haven't tried yet** — access to curated list of quality options
2. **Feel confident in recommendations** — gems are pre-filtered for quality (4.0+ rating)
3. **Explore diverse cuisine & occasion options** — find both casual hangouts and fine dine moments

### Business Goals
1. **Increase dine-out reservations** — surface 200+ high-quality restaurants that were invisible before
2. **Expand addressable restaurant inventory** — reduce reliance on top 50 restaurants (diversification)
3. **Build user engagement & habit** — create "discovery" use case (vs transactional booking)
4. **Differentiate from Zomato** — curation positioning (human-curated gems vs algorithmic popularity sort)

### Success Metrics

| Metric | Target | Rationale |
|--------|--------|-----------|
| **Click-Through Rate (CTR) on Hidden Gems section** | 12% within 60 days of launch | Benchmark: typical platform features get 8-10% CTR; curation should exceed this |
| **Reservation Conversion from Hidden Gems** | 8% (click → reservation) | Baseline for Swiggy is 6-7%; curated content should convert better |
| **Hidden Gems bookings as % of total platform bookings** | 15% within 90 days | Growth metric: ensure hidden gems drive meaningful GMV, not just novelty |
| **Repeat visit rate to Hidden Gems section** | 35% of users return weekly | Engagement metric: show users come back for discovery, not one-time use |

---

## 5. Proposed Solution

### Feature Overview
**"Hidden Gems"** is a dedicated discovery section on Swiggy Dineout featuring high-rated, low-visibility restaurants. It helps users find quality dining options they wouldn't otherwise discover, while expanding Swiggy's restaurant inventory and user engagement.

### How It Works

#### **Hidden Gem Eligibility Criteria (Algorithm)**
A restaurant qualifies as a "Hidden Gem" if:
- ✅ **Rating ≥ 4.0** (high quality, same as Swiggy's "top-rated" standard)
- ✅ **Reviews/Votes < 200** (low visibility — not yet discovered)
- ✅ **Table Booking Enabled** (core to Swiggy Dineout's offering)
- ✅ **Hygiene/Safety Scores ≥ 4.0** (additional quality check)

#### **Ranking/Personalization Logic**
1. **Primary Sort:** Highest rating (descending) — show best hidden gems first
2. **Secondary Sort:** Recency + Freshness — rotate gems weekly to encourage repeat visits
3. **Personalization Inputs:**
   - **Cuisine preference** — if user browsed "Italian" recently, prioritize Italian hidden gems
   - **Price segment** — if user searched ₹300-600 range, show hidden gems in that range
   - **Location** — show hidden gems within user's delivery radius + nearby search history
   - **Occasion** — if user searches "date night," highlight fine dine hidden gems

#### **User Interface**

**Screen 1: Home Feed**
- "Hidden Gems 💎" section appears **below fold** (after main filters, featured restaurants)
- Horizontal scroll card format showing 3-4 visible hidden gems
- Each card displays: restaurant name, cuisine, ⭐4.2 rating, 156 reviews badge, ₹450 cost, "Newly Discovered" badge
- CTA button: "See All" → navigates to Hidden Gems full list page

**Screen 2: Hidden Gems Full List Page**
- Header: "Hidden Gems in Bangalore 💎"
- Subheader: "High-rated restaurants you haven't tried yet"
- Filters: Cuisine | Cost | Distance | Occasion
- Vertical list of 5-6 restaurant cards per page
- Each card: image, name, cuisine tags, ⭐4.2 (156 reviews), ₹450 cost, distance, "Book Table" button

**Screen 3: Restaurant Detail Page**
- Hero image
- "💎 Hidden Gem" badge with tooltip: "Highly rated (4.0+) but less discovered — be one of the first!"
- Restaurant details: name, cuisine, rating, reviews, cost, address, timings
- Prominent "Book a Table" CTA (orange button, 60px height)
- Reviews section (2-3 sample high-quality reviews)
- "Why Hidden Gem?" section explaining: "This restaurant has excellent ratings but isn't yet on everyone's radar — we're bringing it to your attention because it's truly great"

### Edge Cases Handled
- **New restaurant with <200 reviews** → Allow qualification if ≥4.0 rating (encourage early adoption)
- **Seasonal fluctuation** → Refresh hidden gems list monthly to ensure freshness & reduce fatigue
- **Location isolation** → Ensure at least 5-10 hidden gems per location; for underserved areas, expand to nearby areas
- **Hygiene/Safety concerns** → Override eligibility if recent hygiene score drops <3.8

---

## 6. User Stories

1. **As a** weekend casual diner browsing Swiggy Dineout, **I want to** see a curated list of high-rated restaurants with few reviews, **so that** I can discover new places to try with friends without taking a risk on low-quality options.

2. **As a** food explorer, **I want to** filter hidden gems by cuisine (e.g., Continental, Mediterranean) and price segment, **so that** I can discover restaurants matching my specific occasion and preferences.

3. **As a** busy professional, **I want to** see hidden gems personalized by my recent searches and preferences, **so that** I get relevant recommendations without having to scroll through generic lists.

4. **As a** restaurant owner in an emerging location, **I want to** be featured in the Hidden Gems section despite having fewer reviews than popular restaurants, **so that** I get visibility and bookings from Swiggy's quality-conscious users.

5. **As a** Swiggy Dineout power user, **I want to** see the hidden gems section update weekly with new discoveries, **so that** I keep returning to the app for fresh recommendations.

---

## 7. Feature Scope

### In Scope (V1)
1. ✅ Backend algorithm to identify hidden gem restaurants (rating ≥4.0, votes <200, table booking enabled)
2. ✅ Home feed section: "Hidden Gems" carousel with 3-4 visible restaurants
3. ✅ Full list page: all hidden gems in the user's location/delivery radius with basic filters (cuisine, cost)
4. ✅ Restaurant detail page: new "Hidden Gem" badge with explanatory tooltip
5. ✅ Analytics: CTR, conversion, repeat visit tracking for hidden gems section

### Out of Scope (V1 — Future)
1. ❌ AI-based personalization by taste profile (complex NLP on review text) — defer to V2
2. ❌ Social features ("Save Hidden Gems," "Share with friends") — launch as separate feature
3. ❌ Hidden Gems contests/gamification ("Visit 5 hidden gems, get 20% off") — post-launch engagement layer

---

## 8. Edge Cases & Risks

| Edge Case | Risk | Mitigation |
|-----------|------|-----------|
| **New restaurant with <20 reviews but 4.0+ rating** | Too risky — might be fake/biased reviews | Only qualify restaurants with ≥30 reviews (min threshold) to ensure statistical significance |
| **Restaurant with poor hygiene score but 4.0+ food rating** | Violates quality promise; ruins user trust | Add hygiene/safety score filter (≥4.0) to eligibility; override if safety score drops after qualification |
| **Geographic isolation: some areas have <5 hidden gems** | Can't fill "Hidden Gems" section in underserved areas | Expand radius intelligently; show "Nearby Hidden Gems" in adjacent areas; prioritize onboarding more restaurants in underserved areas |
| **Hidden gems become over-promoted → lose "undiscovered" feeling** | Feature loses novelty after 2-3 weeks of use | Rotate gems weekly; show 20-30 gems total, not just top 5 repeatedly; refresh algorithm monthly |

---

## 9. Launch Plan

### Phase 1: Internal Testing (Weeks 1-2)
- QA team validates hidden gem algorithm on staging data
- Design & product review wireframes and interactions
- Run A/B test with internal users (Swiggy employees in Bangalore)
- Collect feedback: UI clarity, algorithm accuracy, personalization relevance
- **Deliverable:** Polished feature, ready for soft launch

### Phase 2: Soft Launch — 10% User Rollout (Weeks 3-4)
- Release Hidden Gems to 10% of Swiggy Dineout Bangalore users (randomly selected)
- Monitor: CTR, conversion rate, repeat visit rate, user feedback
- Set alert thresholds: if CTR <6%, conversion <4%, escalate to product team
- Run daily standups with analytics & support teams to catch issues early
- **Target:** Validate feature viability; collect 500+ bookings data point
- **Deliverable:** Feature usage report, top issues, recommendations

### Phase 3: Full Rollout (Week 5+)
- Roll out to 100% of Swiggy Dineout Bangalore users (if Phase 2 metrics positive)
- Expand to other cities: Delhi, Mumbai, Hyderabad (weeks 6-8)
- Optimize based on learnings: adjust filters, personalization, algorithm weights
- Plan next features: social sharing, hidden gems contests, ratings gamification
- **Target:** Hidden gems to represent 10-15% of total platform bookings within 90 days

---

## 10. Open Questions

1. **Personalization Trade-off:** Should we prioritize hidden gems that match user's recent cuisine searches, or show diverse cuisines to maximize discovery? (Data needed: which approach drives higher conversion + retention?)

2. **Promotion Strategy:** Should hidden gems be "exclusive" (only shown to logged-in Swiggy Dineout premium members) or available to all users? (Trade-off: exclusivity drives engagement but limits reach; accessibility maximizes impact)

3. **Restaurant Partner Incentives:** Should we offer Swiggy Dineout partners a way to "opt-in" to hidden gems feature (e.g., offer a discount on their listing fee), or is organic algorithmic qualification better? (Trade-off: incentives drive quality, but may introduce bias)

---

## Success Definition

**MVP Launch Success:** Feature achieves ≥10% CTR and 6%+ conversion within first 60 days, with zero major bugs or user complaints regarding accuracy of hidden gem recommendations.

---

## Appendix: Supporting Data from EDA

### Hidden Gems Opportunity
- **Inventory:** 200-300 high-quality (4.0+ rating) but low-visibility (<200 votes) restaurants in Bangalore
- **Quality:** Hidden gems have identical avg rating (4.2⭐) as highly-voted restaurants (4.2⭐), but 5-10x fewer visits
- **Cost:** Hidden gems average ₹450-550 for two people (mainstream segment, not premium premium)
- **Distribution:** Hidden gems exist in ALL 50+ locations, with highest concentration in tier-2 areas (underserved neighborhoods)
- **Use Case Fit:** 100% of hidden gems have table booking enabled (perfect for Swiggy Dineout's core offering)

### Market Validation
- Zomato Bangalore delivery-focused (70% of restaurants)
- Swiggy Dineout = pure dine-in play (25-30% of restaurants offer table booking)
- Hidden gems fill the gap: curated, dine-in-only, quality-focused discovery experience