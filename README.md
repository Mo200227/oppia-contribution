# Open Source Contribution Journal — CodePath AI301

## About This Repo
This repository documents my open source contribution journey 
as part of CodePath's AI301 capstone course.

## Issue Selected
**Project:** Oppia  
**What it is:** A free, online learning platform to make 
quality education accessible for all  
**Issue #:** 19610  
**Issue Title:** Add field for developer-supplied notes 
for feature flags  
**Link:** https://github.com/oppia/oppia/issues/19610  
**Labels:** good first issue, Work: Low, Impact: Medium  

## What The Issue Is About
The Oppia platform has "feature flags" — settings that 
developers can turn on/off in the Release Coordinator page. 
Currently these flags have no way to include notes for 
the admins who manage them.

The goal is to add a `developer_notes` field to the feature 
flag specification so developers can write instructions like 
"When this flag is turned off, please click the Regenerate 
summary models button." These notes should appear in the 
Release Coordinator UI when they are not empty.

## Why I Picked This Issue
- Labeled "good first issue" with "Work: Low"
- The solution approach is clearly documented in the 
  issue comments
- Involves Python (backend) which I have experience with
- The task is well-scoped and concrete

## Files I Will Need To Change
Based on reviewing the issue discussion:
- `core/domain/feature_flag_domain.py` — add 
  `developer_notes` field to FeatureFlagSpec
- `core/templates/pages/release-coordinator-page/
  features-tab/features-tab.component.html` — display 
  the notes in the UI
- `core/templates/pages/release-coordinator-page/
  features-tab/features-tab.component.ts` — update 
  the component logic
- Related test files

## My Plan
- [x] Find and select an appropriate issue
- [x] Comment on the issue expressing interest
- [ ] Wait for maintainer confirmation
- [ ] Set up Oppia locally on my machine
- [ ] Reproduce the missing feature
- [ ] Implement the fix
- [ ] Record a demo video
- [ ] Submit pull request

## Status
Currently waiting for maintainer response after 
expressing interest on June 5, 2026.
