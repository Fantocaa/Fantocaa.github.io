# Recruitment Psychotest Platform

A recruitment team needs to invite applicants to take an assessment and then review their results. Applicants need a straightforward test experience, while the people managing questions and reports need a protected workspace. Both sides belong to the same process, but they should not share the same access.

## The problem to solve

Sending someone a test link solves only the invitation. The questions still need to be organized, the applicant needs to move through the test sections, and the result needs to come back in a form a recruiter can actually review or share.

## How I approached it

I built the administrative flow for creating individual test links, managing questions and sections, and reviewing applicant records. Applicants use a public link to start a section and submit answers without entering the administration area. The reporting flow provides detailed and skill-oriented views, controlled links for sharing reports, and a PDF export.

The Laravel backend connects the test, submission, and reporting workflows. React, TypeScript, and Inertia provide the interfaces on both sides. Roles, permissions, and audit logs support the protected administrative work.

## What this delivers

Recruiters have a path from preparing an assessment to reviewing its report. Applicants use a separate route that keeps the administration workspace out of their test experience.

This is the private `module-psychotest` project. Applicant information, test material, and source code are not published here. [Discuss a similar project](mailto:fantocaa17@gmail.com).
