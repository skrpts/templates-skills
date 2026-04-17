---
type: workflow
id: templates-skills
title: "Skill Templates"
description: "Skill templates — processing, content creation, code review, research, and analysis"
tags: [Production, Templates]
connections:
  - target: skill-file-processor
    type: uses
  - target: skill-content-writer
    type: uses
  - target: skill-code-reviewer
    type: uses
  - target: skill-research-analyst
    type: uses
  - target: skill-translator
    type: uses
  - target: skill-data-analyser
    type: uses
  - target: skill-meeting-summariser
    type: uses
  - target: skill-email-drafter
    type: uses
  - target: skill-seo-optimiser
    type: uses
  - target: skill-quality-reviewer
    type: uses
  - target: llm-service
    type: runs_on
metadata:
  estimated_duration: "1 minute"
  trigger: manual
  template: true
output_step: "skill-file-processor"
composite_steps:
  - "skill-file-processor"
  - "skill-content-writer"
  - "skill-code-reviewer"
  - "skill-research-analyst"
  - "skill-translator"
  - "skill-data-analyser"
  - "skill-meeting-summariser"
  - "skill-email-drafter"
  - "skill-seo-optimiser"
  - "skill-quality-reviewer"
execution:
  - skill: "skill-file-processor"
    step_type: "generation"
---

## Overview

This skrpt contains 10 skill templates for use when creating new skill nodes. Import this skrpt to add these templates to your template picker.

## Templates

### Processing

- **File Processor** — Processes an uploaded file and extracts structured content
- **Document Translator** — Translates content between languages while preserving formatting
- **Data Analyser** — Analyses datasets and produces insights
- **Meeting Summariser** — Summarises meeting transcripts into structured notes
- **Quality Reviewer** — Reviews output against defined quality criteria

### Content

- **Content Writer** — Generates written content from a topic and brief
- **SEO Optimiser** — Optimises content for search engine visibility

### Development

- **Code Reviewer** — Reviews source code for quality, security, and best practices

### Research

- **Research Analyst** — Analyses a topic and produces structured research findings

### Communication

- **Email Drafter** — Drafts emails from context and intent

