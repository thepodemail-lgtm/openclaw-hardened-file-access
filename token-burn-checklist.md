# Token-Burn Checklist — set these 5 before your agent runs free

An agent left running with no caps will, sooner or later, loop — and a loop
burns tokens and money while nobody is watching. These five caps and checks
take about ten minutes to set and turn that surprise into a small, logged
event. Set all five before you let any agent run on its own.

## 1. Daily token cap

Set a hard total for one calendar day, sized to your real budget — not to
your best day. When the day's total is hit, calls stop until tomorrow.
Rule of thumb: pick the number you would be annoyed, not hurt, to spend in
one bad day.

## 2. Hourly token cap

A daily cap alone still lets a bad hour burn the whole day. Add an hourly
cap (tokens in the last 60 minutes) well below the daily one. A healthy
agent almost never comes close; a looping one hits it fast.

## 3. Loop limit

Caps count tokens; a loop limit counts calls. Set a max number of model
calls inside a short window (60 seconds is a good start — 30 calls is a
generous ceiling for most personal agents). A real task breathes between
calls. A loop does not. This is the check that catches a runaway first.

## 4. An alert you will actually see

A cap that trips silently is only half a guard. Make every trip write
something you check daily: an alert file on your desktop, a line in a log
you read with your morning coffee, a message to yourself. Name the cap and
the time in the alert, so the next morning you know what happened without
digging.

## 5. A sandbox test before live trust

Never test caps on a live agent with a live key. Run fake calls first with
tiny test caps and watch each cap trip on purpose: calls stop, the error is
clear, the log line and the alert appear. Only then point the real agent at
the real limits — with the caps set below the most you are willing to
spend, because calls already made are already billed.

