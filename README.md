# Unclosed HTML Tag Bug

This repository demonstrates a subtle bug related to using `innerHTML` in JavaScript to modify HTML content.  The issue stems from an unclosed paragraph tag (`<p>`) within the string assigned to `innerHTML`. This can lead to unexpected rendering or even script errors, depending on the browser's HTML parsing behavior.

## Bug Description
The provided HTML file uses `innerHTML` to insert a paragraph into a div. However, the paragraph tag is not properly closed, potentially causing incorrect rendering or unexpected behavior.  Modern browsers might try to recover and still display the content, but this is not guaranteed and could lead to inconsistencies across different browsers.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe the unexpected display or behavior (likely missing or malformed text).

## Solution
The solution involves correctly closing the paragraph tag within the `innerHTML` string. This ensures the HTML is valid and renders as expected.
