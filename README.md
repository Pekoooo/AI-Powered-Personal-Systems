# AI-Powered Personal Coaching System
**Prompt Engineering | MCP Integration | Multi-Database Coordination**

A production-grade AI coaching system built with Claude AI, demonstrating advanced prompt engineering, database integration via Model Context Protocol (MCP), and real-time state management across multiple Notion databases.

##  Project Overview

Personal workout and nutrition coaching system that automatically tracks macros, logs meals, monitors progress, and coordinates state across 7 interconnected Notion databases. Built to solve real tracking friction with intelligent automation and visual feedback.

**Core Problem Solved**: Eliminated manual nutrition tracking overhead while maintaining data accuracy and cross-system coordination for comprehensive personal analytics.

##  Technical Architecture

### System Components
```
User Input → Claude AI (Custom Instructions) → MCP Protocol → Notion API
                    ↓
        Multi-Trigger State Management
                    ↓
    ┌───────────────┴───────────────┐
    ↓                               ↓
Database Queries              Real-Time Updates
    ↓                               ↓
ASCII Visualization          Cross-System Sync
```

### Key Technologies

- **AI Platform**: Claude AI with custom instruction architecture
- **Integration Protocol**: Model Context Protocol (MCP) for Notion
- **Database**: 7 interconnected Notion databases
- **State Management**: Trigger-based update system with cross-project coordination
- **Visualization**: Real-time ASCII progress bars with percentage calculations

##  Database Schema Design

### Coordinated Databases

1. **Central Life Dashboard** - Master state coordinator
   - Tracks: Weight trends, energy levels, training frequency
   - Purpose: Cross-AI-project synchronization hub

2. **Nutrition Database** - Food library (100+ items)
   - Fields: Calories, protein, carbs, fat, fiber, sugar per serving
   - Auto-queried before calculations

3. **Daily Meal Log** - Consumption tracking
   - Combined meal entries with ingredient breakdowns
   - Automatic macro totals and goal progress

4. **Weight Log** - Progress tracking
   - Auto-calculated daily changes
   - Trend analysis integration

5. **Body Measurement Database** - Physique tracking
   - Key ratios: Chest-to-waist, shoulder-to-waist
   - Progress toward aesthetic benchmarks

6. **Workout Journal** - Training consistency
   - Session logging and pattern analysis

##  Prompt Engineering Architecture

### Multi-Layer Instruction System

**Layer 1: Core Behavior Rules**
- Cooking method assumptions (auto-add olive oil)
- Protein quality validation (70% complete protein rule)
- Macro priority hierarchy (carbs-first approach)

**Layer 2: Trigger-Based State Management**
```
IF user logs weight
  → UPDATE Central Dashboard: Current Weight, Weight Trend
  → QUERY Weight Log for previous entry
  → CREATE new entry with auto-calculated change
  → ANALYZE trends and provide insights
```

8 distinct triggers managing cross-database updates and state synchronization.

**Layer 3: Workflow Protocols**
- Meal Logging: 11-step process from database query to visualization
- Weight Tracking: 6-step process with trend analysis
- Daily Intake Analysis: 7-step process with compliance scoring

**Layer 4: Quality Assurance**
- ASCII visualization accuracy requirements
- Mandatory calculation verification steps
- Database query priority over general knowledge

### Example Trigger Implementation
```
TRIGGER 1: User logs new weight
→ UPDATE: Current Weight (kg)
→ UPDATE: Weight Trend
→ UPDATE: Last Weight Update
→ UPDATE: Last Updated By: "Workout Coach"
→ CROSS-REFERENCE: Previous day weight for delta calculation
```

##  Real-Time Visualization System

### ASCII Progress Bar Engine

Implements precise percentage-to-character conversion:
```
Calculating: 2400/2800 = 85.7% → 85.7 × 20 = 17.14 → 17 filled characters

Calories: [█████████████████░░░] 2400/2800 (86%)
Protein:  [██████████████░░░░░░] 112/140g (80%)
Carbs:    [███████████░░░░░░░░░] 200/350g (57%) ⭐
Fat:      [████████████████░░░░] 80/120g (67%)
Fiber:    [██████░░░░░░░░░░░░░░] 14/35g (40%)
```

**Technical Requirements:**
- Exactly 20 characters per bar
- Formula: `(current / target) × 20`, rounded to nearest integer
- Mandatory pre-calculation verification step
- Dynamic target handling (e.g., 300-400g carb range = 350g midpoint)

##  Advanced Features

### 1. Screenshot Recognition Workflow
- Extract nutrition data from images
- Confirm product identification
- Add to database (NOT auto-log as consumed)
- Maintain separation between library and consumption

### 2. Protein Quality Validation
- Minimum 70% complete protein per meal
- Automatic flagging of insufficient quality
- Complete vs incomplete protein classification

### 3. Cross-Project State Coordination
- "Last Updated By" tracking prevents circular updates
- Shared problem area management
- Energy level and compliance scoring across AI assistants

### 4. Intelligent Query Protocol
```
Priority Order:
1. Check Central Dashboard for current state
2. Query relevant Notion database
3. Use general knowledge for estimates (last resort)
4. Update Central Dashboard if triggers met
```

##  Real-World Impact

**Tracking Automation:**
- 2,800 daily calories monitored across 4 macronutrients
- 100+ food items in searchable nutrition database
- 7 interconnected databases coordinated in real-time

**Data Accuracy:**
- Automatic cooking oil inclusion (14-21g fat per meal)
- 70% complete protein validation on every meal
- Cross-referenced database queries before estimation

**User Experience:**
- Visual progress feedback on every interaction
- Proactive macro balance recommendations
- Single confirmation for dual action (calculation + logging)

##  Technical Challenges Solved

1. **State Synchronization**: Trigger system prevents data conflicts across multiple AI assistants
2. **Calculation Accuracy**: Mandatory verification steps for ASCII visualizations
3. **Query Optimization**: Database-first approach reduces hallucination risk
4. **Context Management**: Long conversation reminders maintain instruction adherence
5. **User Friction Reduction**: Screenshot parsing, auto-assumptions, combined logging

##  Skills Demonstrated

**AI & Prompt Engineering:**
- Complex multi-layer instruction architecture
- Conditional logic and trigger-based workflows
- Long-form context management and reminder systems

**System Integration:**
- MCP protocol implementation for Notion API
- Multi-database coordination and state management
- Real-time data synchronization

**Data Architecture:**
- Relational database schema design
- Cross-table referencing and data integrity
- Query optimization and priority protocols

**Software Engineering Principles:**
- Modular workflow design (11-step meal logging process)
- Error prevention through mandatory verification
- User-centric automation (reduce friction, maintain control)

  ## Key Learnings

1. **Prompt Engineering is System Design**: Treating AI instructions like software architecture produces reliable, maintainable systems
2. **State Management Matters**: Cross-context coordination requires explicit trigger protocols
3. **Database-First Reduces Hallucination**: Priority query systems improve accuracy
4. **Verification Layers Build Trust**: Mandatory calculation checks prevent compounding errors
5. **User Friction = Adoption Barrier**: Smart defaults and auto-assumptions drive consistent usage

##  Related Experience

This project applies software engineering principles from my Android development background:
- **Clean Architecture thinking** → Layered prompt instruction design
- **State management patterns** → Trigger-based update system
- **API integration experience** → MCP protocol implementation
- **Real-world problem solving** → Building tools that eliminate friction

---

**Built by Clément Le Corre** | [GitHub](https://github.com/Pekoooo) | [Medium](https://medium.com/@clec.78)

*Demonstrating practical AI integration, system design, and prompt engineering for real-world applications.*
