# Code Review Guidelines

## Purpose

This document provides practical guidelines for reviewing code in a technical team.

The goal of code review is not only to find defects. It is also to improve maintainability, share knowledge, reduce risk, and align the team around quality standards.

## What to Review

### 1. Business Logic

- Does the change solve the expected problem?
- Is the logic aligned with the business requirement?
- Are edge cases considered?
- Is the behavior easy to understand?

### 2. Readability

- Is the code easy to read?
- Are names clear and meaningful?
- Is the structure simple?
- Is unnecessary complexity avoided?

### 3. Maintainability

- Can another developer understand and modify this later?
- Is the code organized in a reasonable way?
- Are responsibilities separated?
- Is duplicated logic avoided?

### 4. Testing and Validation

- Was the change tested?
- Are important scenarios covered?
- Are failure cases considered?
- Is there evidence of validation?

### 5. Security and Privacy

- Are credentials, tokens, or secrets excluded?
- Is sensitive information protected?
- Are inputs validated?
- Are permissions and access controls considered?

### 6. Documentation

- Was documentation updated if needed?
- Are important decisions explained?
- Is the README or related documentation still accurate?

## Review Mindset

A good code review should be:

- Respectful
- Clear
- Practical
- Focused on the work, not the person
- Oriented toward improvement
- Aligned with team standards

## Reviewer Checklist

- I understand the purpose of the change.
- I reviewed the main logic.
- I checked for obvious risks.
- I checked for sensitive information.
- I considered maintainability.
- I reviewed testing evidence.
- I left clear comments where needed.
- I can approve this change with confidence.

## Contributor Checklist

Before requesting review, the contributor should confirm:

- The change is ready for review.
- The branch is up to date.
- The code was tested.
- The pull request description is complete.
- The scope is controlled.
- No sensitive information was included.

## Common Review Comments

Examples of useful review comments:

```text
Can we simplify this logic?
Could this validation be reused?
What happens if this value is empty?
Can we add a short explanation here?
Is this behavior covered by a test?
Could this expose sensitive information?
```

## Final Principle

Code review is a quality practice and a collaboration practice.

The objective is to help the team deliver better software with less risk and more shared understanding.
