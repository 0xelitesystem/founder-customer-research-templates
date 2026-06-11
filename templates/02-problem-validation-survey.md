# 02. Problem validation survey

## Goal

Test a problem hypothesis at scale (50-500 responses) after you have qualitative signal from interviews. The survey is not for discovery. If you don't already know roughly what the problem looks like, run interviews first.

Walk away with:
- How many people in your target segment experience the problem
- How they currently solve it
- How painful it is (with a number you can rank)
- Who to interview next

## Length

8 questions maximum. Every additional question drops response rate. If you're tempted to add a tenth question, ask which of the existing nine you can cut.

## Distribution

Send via direct outreach (one-to-one email or LinkedIn message), not mass blast. Personalize the first sentence. Response rates on personalized outreach run 15-30 percent; mass blasts run 1-3 percent and the responders are unrepresentative.

## Template

### Intro line (above the questions)

> Quick 3-minute survey for [target audience]. I'm researching how teams handle [problem area]. No marketing follow-up, no product pitch. Results will be shared back with respondents who want them.

### Question 1: Qualifying

**Are you currently [doing the thing the problem affects]?**
- Yes, daily or weekly
- Yes, occasionally
- No

If "No", skip to question 8.

### Question 2: Frequency

**In the past 30 days, how often did [specific situation] happen?**
- 0 times
- 1-3 times
- 4-10 times
- More than 10 times

Avoid Likert scales for frequency. Numbers are more honest.

### Question 3: Current solution (open-ended, short)

**The last time [specific situation] happened, how did you handle it? Be specific. Tools, people, steps.**

This is the most valuable question. Read every answer.

### Question 4: Friction (open-ended, optional)

**What was the most annoying part?**

Optional means optional. Don't make it required, or you'll get "nothing" and "n/a".

### Question 5: Spend

**Does your team currently pay for any tools to help with this?**
- Yes, list them: ___
- No, but we've considered it
- No, not relevant to pay for

### Question 6: Severity (one number)

**On a scale of 1 to 10, how much does [problem] affect your work?**
- 1 = doesn't really
- 10 = blocking my work regularly

A single 1-10 scale beats five Likert questions. People can rank themselves on one axis honestly. They can't rank themselves on five.

### Question 7: Search behavior

**Have you searched for a solution to this in the last 90 days?**
- Yes (what did you search for? ___)
- No, hadn't thought to look
- No, I assume no good solution exists

### Question 8: Follow-up consent

**Can I email you a few follow-up questions in the next 2 weeks?**
- Yes (email: ___)
- No

That's it. 8 questions, 3 minutes.

## Anti-patterns

| Bad question | Why it's bad |
|--------------|--------------|
| "How interested are you in a tool that ___?" | They'll say "very" to be polite. Means nothing. |
| "How much would you pay for ___?" | They have no idea. Their number is a guess. |
| "Rate the following features by importance" | Everything will come back rated 4-5 out of 5. Forced ranking is better, but takes longer. |
| "Tell us about yourself" with 6 demographic fields | Cuts response rate. Ask demographics only if you'll segment on them. |
| "What's your role?" with 20 dropdown options | Use 5 broad buckets. You don't need to distinguish "Senior PM" from "Staff PM" for this survey. |

## Analysis

Don't compute means on Question 6 right away. First, look at the distribution.

- If most answers are 1-4: the problem isn't painful enough. Don't build.
- If most are 8-10: there's a real problem. Read every open-ended answer.
- If it's bimodal (cluster at 2 and cluster at 9): there are two segments. Figure out what differentiates them; that's your initial customer.

Read every Question 3 (current solution) answer. Look for:
- Specific tools mentioned (these are your competitors)
- "Spreadsheet" or "email thread" (good signal: a real workaround that doesn't scale)
- "We don't really handle it" (great signal: ignored problem)

## What to do with the data

1. Pull contact info from anyone who answered 8+ on Q6 AND opted into Q8 follow-up. Interview them next (use template 01).
2. Save the verbatim language from Q3 and Q4. This is landing page copy.
3. Note the tools mentioned in Q5. These are your competitors and your potential integration partners.
4. If 80%+ of responses say "no I haven't searched" on Q7, your problem may not be top-of-mind. Reconsider before building.
