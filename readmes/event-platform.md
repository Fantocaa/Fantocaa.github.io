# Multi-Tenant Event Platform

The platform operator serves multiple event organizers. Each organizer needs a place to manage its events and guests, while the operator needs to create and administer those separate workspaces. Mixing both responsibilities in one shared data space makes it hard to know which organization's records a request belongs to.

## The problem to solve

The difficult part was the boundary between platform administration and an organizer's day-to-day work. A new organizer needed a usable workspace, not just an account. Once that workspace existed, its event data had to stay tied to the right organization on every request.

## How I approached it

I separated the central tenant and access records from the event and guest records owned by each tenant. A subdomain identifies the organizer's context; its own PostgreSQL database holds its operational data. I also connected tenant creation to database setup, migrations, and initial roles and menus, so provisioning a workspace prepares the application to be used.

Laravel handles the tenant lifecycle and requests, while React and Inertia provide the interface. Redis supports sessions, caching, and queued work. Those tools serve the underlying decision: shared platform administration, separate organizer workspaces.

## What this delivers

The operator can set up and manage organizations without putting their event data in the shared administrative space. Each organizer works with its own events and guests through its own subdomain.

This is a private project. Client records, internal configuration, and source code are not published here. [Discuss a similar project](mailto:fantocaa17@gmail.com).
