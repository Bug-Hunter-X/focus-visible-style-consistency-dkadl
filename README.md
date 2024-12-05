# :focus-visible Pseudo-class Issue

This repository demonstrates a bug where the CSS `:focus-visible` pseudo-class is not consistently applying styles across different browsers.  The issue is particularly noticeable in [Browser Name and Version].  The `focus-bug.css` file contains the problematic code, while `focus-solution.css` offers a potential solution.

## Problem

The expected behavior is that when an element receives focus, the styles defined within the `:focus-visible` rule should only be applied if the focus is not programmatically triggered (e.g., by JavaScript).  However, in the affected browsers, these styles are not applied, even when the focus is user-initiated. 

## Solution

The solution involves using JavaScript to explicitly manage focus and apply styles accordingly. This may include using additional CSS classes or JavaScript event listeners to handle user-initiated focus.