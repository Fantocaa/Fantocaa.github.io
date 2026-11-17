# Wedding Invitation & RSVP

A couple needs an invitation that feels personal to each guest, and a practical way to know who plans to attend. Making a separate page for every person would be cumbersome to maintain; collecting replies without a guest list would leave the organizers doing the matching by hand.

## The problem to solve

The public invitation and the private guest list have different jobs. Guests should be able to open their invitation and reply easily on a phone. The organizer needs to manage guest records and see attendance status without exposing that information to everyone visiting the page.

## How I approached it

I built one invitation experience that looks up a guest by an individual invitation code. That lets the page show a personalized invitation and connect its RSVP to the right record. A protected dashboard handles guest creation, edits, invitation codes, and attendance tracking. The public page and the administrative work share the same application data without sharing the same access.

Next.js and React provide the invitation and dashboard; TypeScript covers the interface and server routes, with Supabase supporting the data layer. The central decision is using one maintained invitation experience with guest-specific access, rather than duplicating pages.

## What this delivers

Guests have a direct way to view and answer their invitation, while the organizers can follow responses in one place. This is a private project; guest details, invitation codes, and source code are not published here. [Discuss a similar project](mailto:fantocaa17@gmail.com).
