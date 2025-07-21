# Email Analyzer: Psycholinguistic Diagnostic Tool

_A diagnostic tool that empowers users with shareable reports exposing manipulative institutional language, while aggregating patterns across organizations to drive transparency and collective accountability._

## Overview

Subject is an email analysis tool designed to diagnose and expose subtle forms of manipulation, ambiguity, and accountability avoidance in institutional email communication. The tool generates shareable reports and aggregates findings to create a single, central source of truth for organizational accountability.

## How It Works

- Users submit institutional emails for analysis.
- The tool applies advanced psycholinguistic analysis to identify patterns of manipulation, passive-aggressiveness, ambiguity, lack of transparency, and credibility issues.
- Results are presented in a clear, shareable report, and aggregated to reveal broader patterns across organizations.

## Live Demo

**[Explore the Email Analyzer Demo](https://email-analyzer-nine.vercel.app/)**  
*(The demo highlights key features — AI-driven tone analysis, psycholinguistic scoring, and shareable reports — powered by mocked data to simulate real-world email patterns.)*

## Portfolio Article

For a detailed look at the concept, design process, and future roadmap of the Email Analyzer, read the full portfolio article:

[**Read the Portfolio Article**](https://www.notion.so/Why-I-built-Subtext-Exposing-Accountability-Avoidance-in-Email-2351d53cfded80d38651e95f3047caaf)

## Current Development & Prompt Engineering

The Email Analyzer is still in active development, with a focus on refining the AI prompt to deliver more accurate and consistent scoring. While the core UI and scoring framework are complete, the underlying analysis logic is being iterated to better detect nuanced communication patterns. Updates will include:

- Improved prompt calibration for subtle accountability avoidance.
- More robust scoring logic (exploring non-linear models).
- Expanded example cases to test reliability across varied writing styles.

## Screenshots

**Landing Page/Email Input**
[Email Input Screenshot](https://github.com/vwvw25/email-analyzer/blob/main/screenshots/Screenshot%202025-07-21%20at%2000.42.10.png)

**Report Page** 
[Report Page Screenshot](https://github.com/vwvw25/email-analyzer/blob/main/screenshots/Screenshot%202025-07-21%20at%2000.41.51.png)  

## Project Architecture

The Email Analyzer uses the Next.js 13+ App Router structure, featuring serverless API routes, dynamic report pages, and top-level layout components.

```
email-analyzer/
├── public/
│   ├── .svg                # Icons
│   ├── grain.1ccdda41.png   # Background texture
│   └── subtext-logo.       # Logo files
├── src/
│   └── app/
│       ├── api/
│       │   └── analyze/
│       │       └── route.ts          # API endpoint for email analysis
│       ├── privacy-policy/
│       │   └── page.tsx              # Privacy policy page
│       ├── report/
│       │   └── [id]/
│       │       └── page.tsx          # Dynamic report pages
│       ├── terms-of-use/
│       │   └── page.tsx              # Terms of use page
│       ├── Footer.tsx                # Footer component
│       ├── Header.tsx                # Header component
│       ├── globals.css               # Global styles
│       ├── layout.tsx                # Root layout
│       └── page.tsx                  # Entry page
├── package.json                       # Project dependencies
├── tsconfig.json                      # TypeScript configuration
└── next.config.ts                     # Next.js configuration
```

## Tech Stack

- **Framework:** Next.js 15 with React 19  
- **Styling:** TailwindCSS  
- **TypeScript:** Full type safety throughout the application  
- **AI/NLP:** OpenAI GPT-4 for psycholinguistic analysis (see `src/app/api/analyze/route.ts:80`)  
- **Data Storage:** In-memory store for MVP (not static JSON files) — see `src/app/api/analyze/route.ts:5`  
- **Hosting:** Vercel  

The project uses OpenAI's GPT-4 model to perform advanced tone and manipulation detection, while results are stored temporarily in memory for rapid prototyping and demo purposes.

## About This MVP

This demo highlights the Email Analyzer’s key capabilities:  
- **Tone & Manipulation Detection:** Identifies passive-aggressive phrasing, ambiguity, and accountability avoidance.  
- **Scoring & Transparency Reports:** Aggregates analysis into shareable reports for institutional review.  
- **Psycholinguistic Insights:** Uses advanced NLP techniques to detect subtle emotional and tonal cues.

The MVP uses mocked data to demonstrate the interface, scoring logic, and reporting format.

## Product Roadmap

### **MVP**
- **Single Email & Thread Analysis:** Users can submit individual emails or threads to receive a detailed, scored report. Reports can be saved or shared for transparency and accountability.

### **Thread-Level Insight**
- **Conversation Dynamics:** Provides full analysis across entire email chains, highlighting tone shifts, escalation points, avoidance tactics, and communication pattern changes over time.

### **Institutional Dashboards**
- **Organization-Wide Trends:** Aggregates anonymized data from user submissions to generate dashboards once a threshold is met. Institutions can view trends, respond to feedback, and monitor patterns of communication over time.

### **Suggested Replies**
- **AI-Generated Counterframes:** Creates tailored reply drafts that address tone issues, evasiveness, or content gaps in the original email. These are not generic templates but context-aware responses aimed at fostering clarity and accountability.

### **B2B Outbound Scoring Tool**
- **Pre-Send Analysis for Institutions:** A SaaS tool enabling organizations to score and refine their outgoing emails. It flags issues such as vagueness, passive aggression, or overly formal language, catering to legal, HR, and customer support teams.

### **Autonomous Complaint Handling**
- **AI Advocacy Agent:** An autonomous agent that manages a user’s complaint end-to-end. It gathers relevant emails, asks clarifying questions, drafts and sends responses, escalates when needed, and tracks outcomes — acting as a delegated advocate for the user.

## About This Project

This project was conceived and built by **Victoria Ward**, combining expertise in psycholinguistic analysis, language bias detection, and AI-powered tooling to create a platform for accountability and communication clarity.
