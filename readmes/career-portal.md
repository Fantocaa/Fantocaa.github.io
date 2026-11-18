# Career & Recruitment Portal

A company needs more than a page announcing that it is hiring. Candidates need to find an opening, understand the role, and reach the right application form. Others may want to send a CV even when they are not applying to a particular vacancy. The portal brings those journeys together with the company's career information.

## The problem to solve

Vacancies are structured records, but candidates experience them as a sequence of pages and decisions. If the listing, role details, and application form do not connect clearly, people can lose their place before applying. The general CV route also needs to make sense alongside applications tied to a specific opening.

## How I approached it

I connected the vacancy listing to individual role pages and application forms for jobs and internships. A separate CV submission route covers candidates without a selected vacancy. Company information, FAQs, and contact pages give people context as they move through the portal. Vacancy URLs use public identifiers rather than exposing raw database IDs.

Laravel manages the vacancy and application data; Inertia connects it to the React pages. The engineering work is in keeping the public journey aligned with those records, so a person can move from discovery to an appropriate form.

## What this delivers

Candidates can move from a vacancy listing to its application form, or choose the general CV route when there is no particular opening they want to apply for.

[Visit the career portal](https://karier.tako.co.id/). This private project is self-hosted on a private company server. Candidate records and source code are not published here. [Discuss a similar project](mailto:fantocaa17@gmail.com).
