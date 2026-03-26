Perfect setup! Here's the plan:
We'll build a Safari Web Extension from scratch with rule-based spam heuristics now, with the architecture ready to drop in your TF.js LSTM model later.
The structure will be:

Xcode Safari Web Extension project (Swift wrapper + web extension target)
Content script injecting into mail.google.com
MutationObserver watching Gmail inbox rows
Rule-based classifier (keyword lists, sender patterns, suspicious URL detection)
DOM highlight engine (green/yellow/red rows + tooltips)
Popup dashboard (stats + threshold controls)