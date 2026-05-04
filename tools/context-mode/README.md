# context-mode

## Problem
Raw outputs (logs, GitHub data) are directly injected into context, bloating it heavily.

## What it does
Stores outputs in SQLite instead of feeding them into the model context directly.

## Impact
~98% reduction in context usage for logs & external data

## Link
https://github.com/mksglu/context-mode
