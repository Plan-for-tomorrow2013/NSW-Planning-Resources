# PFT_OPERATING_SYSTEM

## Purpose

This document is the source of truth for how Plan for Tomorrow stores information, manages workflows, structures knowledge and designs automation.

Where conflicts occur between workflow memory, conversation history, folder structures or automation logic, this document takes precedence.

## 1. Core Principles

### 1.1 Separate Resources from Process

Maintain a clear distinction between:

#### Legislative Resources

NSW planning controls and supporting documents.

Examples:

- Acts
- Regulations
- SEPPs
- LEPs
- DCPs
- Planning Circulars
- Ministerial Directions
- Council Policies

These are reference material.

#### PFT Intellectual Property

How PFT performs work.

Examples:

- Work instructions
- Assessments
- Checklists
- Templates
- Prompts
- Standard responses
- Workflows
- Training material

These are business assets.

#### Project Files

Actual project work.

Examples:

- Client reports
- Development applications
- CDC assessments
- Consultant reports
- BASIX assessments

These are project deliverables.

## 2. Folder Structure

### 00 NSW-Planning-Resources

**Purpose:**

Store planning legislation and supporting materials.

**Contains:**

- PDF versions
- Markdown versions
- Resource databases
- Council planning controls
- LEPs
- DCPs
- SEPPs
- State planning documents

**Notes:**

- This is reference material only.
- No PFT workflows or work instructions are stored here.

### 01 Business Operations

**Purpose:**

Store how PFT operates.

This folder contains:

#### Operating System

Including:

```text
PFT_OPERATING_SYSTEM.md
```

#### Work Instructions

Examples:

```text
How to do a General Enquiry.md
How to complete an Initial Assessment.md
How to start a New Project.md
How to undertake a CDC Assessment.md
How to undertake a DA Assessment.md
How to prepare a SEE.md
How to manage a Refusal.md
```

#### Internal Procedures

Examples:

```text
Project Intake
Quality Assurance
Training
File Management
Automation Workflows
Business Systems
```

**Notes:**

- This folder contains PFT intellectual property.
- Nothing in this folder belongs in NSW Planning Resources.

### 02 Templates, Reference & Knowledge

**Purpose:**

Store tools used to perform work.

#### Templates

```text
SEE Templates
Proposal Templates
Certificate Templates
Email Templates
Assessment Templates
```

#### Knowledge

Examples of good work.

```text
Good SEE examples
Good Objection responses
Good Initial Assessments
Good Planning Reports
```

#### Reference Material

Internal guidance used during delivery.

**Notes:**

- This folder contains working material.
- It is not project specific.

### 03 BASIX & NatHERS

**Purpose:**

BASIX and NatHERS operate as a specialist workflow.

#### Working Documents

- BASIX templates
- BASIX commitments
- NatHERS commitments
- BASIX training material

#### Project Work

Actual BASIX and NatHERS project folders.

**Notes:**

- BASIX/NatHERS is treated as a distinct service line.
- Workflow is separate from CDC and DA planning workflows.

### 04 Clients

**Purpose:**

Work undertaken for external planning businesses.

Examples:

```text
Urban Consultants
Pac Planning
CityPlan
Watermark Planning
```

**Contains:**

- Client projects
- Client templates
- Client specific requirements

**Notes:**

- These are not PFT projects.
- They are projects completed on behalf of other planning consultants.

### 365

**Purpose:**

Workflow development and testing environment.

**Contains:**

- Power Automate
- Copilot
- Power Apps
- AI Experiments
- Workflow Testing

**Notes:**

- No production project material should rely upon the 365 folder.
- Used for testing and development.

## 3. Council Structure

Following migration of LEPs and DCPs to NSW-Planning-Resources:

Council folders contain project work only.

Structure generally follows:

```text
Council
    ↓
CDC or DA
    ↓
Development Type
    ↓
Project
```

Examples:

```text
Blacktown
    CDC
        Secondary Dwelling
        Dual Occupancy
    DA
        Medical Centre
        Child Care
```

Area based grouping may be used where appropriate.

## 4. Markdown Strategy

All operational markdown files are copied to:

```text
Local C Drive
```

for use in:

- VS Code
- Cursor
- Claude
- Git repositories
- AI workflows

OneDrive remains the master business repository.

Git remains an AI/application repository.

## 5. Project Classification Model

Future PFT project creation follows:

```text
Client
    ↓
Council
    ↓
Approval Path
    • CDC
    • DA
    ↓
Development Type
```

Examples:

```text
PFT
    ↓
Canterbury-Bankstown
    ↓
DA
    ↓
Medical Centre
```

```text
PFT
    ↓
Blacktown
    ↓
CDC
    ↓
Secondary Dwelling
```

Automation, templates, workflows and task generation should ultimately be driven from this structure.

## 6. Process Documentation Standard

Every business process will have:

### Human Version

Plain English procedure for staff.

Example:

```text
How to Start a New Project
```

### Markdown Version

Machine readable procedure.

Example:

```text
How_to_Start_a_New_Project.md
```

Both versions must remain aligned.

The markdown version is the workflow source of truth for automation, Copilot, Claude and future AI systems.

This is the first version I'd freeze and put into:

```text
01 Business Operations\PFT_OPERATING_SYSTEM.md
```

Then whenever we design a workflow, such as the New Project Power Automate process we've just built, we update this document first and then create the corresponding human-facing work instruction under Business Operations.
