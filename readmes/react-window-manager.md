# React Window Manager

Some applications need users to keep several pieces of work open at once: moving between panels, comparing information, and returning to a layout they have arranged. A conventional page layout does not offer that kind of workspace. This open-source component gives React applications a way to use movable windows without each app rebuilding the interaction model.

## The problem to solve

Dragging a panel is only one part of a believable window system. Resizing needs limits; overlapping windows need a sensible order; snapping needs to show where a window will land; and minimizing should not make the work disappear. Those behaviours also need to remain coordinated when the application is refreshed or used on a smaller screen.

## How I approached it

I kept window behaviour in a reusable component, separate from whatever content an application puts inside each window. It handles drag and resize interactions, edge snapping into full, half, or quarter-screen layouts, and a preview before docking. Minimized windows move into a reorderable dock. Keyboard actions and mobile swipe gestures cover other ways to manage the workspace, while local storage preserves the arrangement.

React and Zustand support the component and its workspace state. The point of the package is the interaction it provides to the application using it.

## What this delivers

Developers can place their own screens inside the windows and give users a workspace they can arrange and return to. The [public GitHub repository](https://github.com/Fantocaa/winmgr) contains the component and integration details.
