# Goravel + Inertia + React

Starting a new web application often means rebuilding the same foundation before working on the product itself: sign-in, protected pages, account settings, navigation, and a dashboard. I made this open-source starter kit so those pieces could work together from the beginning in a Go and React application.

## The problem to solve

A login screen on its own is not a usable foundation. The server needs to know which routes require a session, the interface needs the current user and validation errors, and people need a place to manage their account. If these pieces are assembled separately, each new app has to resolve the same connections again.

## How I approached it

I used Goravel for the Go backend and Inertia to connect server responses to React and TypeScript pages. The starter includes registration and sign-in, session-based route protection, profile and password settings, and shared authentication and flash-message data. The interface supplies a responsive sidebar, theme switching, and an example analytics dashboard.

The dashboard uses demo figures to show how the interface works.

## What this delivers

A developer can start with an application whose basic account and administration flows are already connected, then replace the example screens with the workflows their own product needs. The [public GitHub repository](https://github.com/Fantocaa/goravel-inertia-react) contains the source, setup instructions, and license.
