---
type: skill
id: skill-file-processor
title: "File Processor"
description: "Processes an uploaded file and extracts structured content"
tags: [Production, Template]
connections: []
metadata:
  template_category: "Processing"
---

Process the following document and extract its content into clean, structured markdown:

{{input.file}}

## Requirements
- Preserve all headings, lists, and tables
- Convert any visual elements to descriptive text
- Maintain the original document structure
- Output clean markdown suitable for further processing
