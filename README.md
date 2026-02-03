# Regex-detects-raw-signals
I built a small system to explore the classic “you can’t regex HTML” problem.
Not to disprove it — but to design around it correctly.
Regex detects raw signals.
A DOM parser provides structure.
A mediation layer reconciles the two and reports where they disagree.
The interesting part isn’t that it works.
It’s that it reveals where parsers silently fix, hide, or merge parts of the original HTML.
The system can now show: • where text and DOM agree
• where the DOM discards things (like script content)
• where malformed HTML gets normalized
• where multiple raw signals map to one structural node
It turns a famous theoretical warning into a visible diagnostic tool
