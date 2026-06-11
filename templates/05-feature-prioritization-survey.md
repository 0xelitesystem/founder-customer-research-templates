# 05. Feature prioritization survey

## Goal

You have 10-50 ideas in a backlog and one engineer (or one quarter of engineering capacity). You want input from real customers on which ones matter. The trick: most prioritization surveys produce garbage data because everyone rates everything as "important".

This template uses two techniques that give honest answers:

1. **Forced ranking** with a hard cap (you must pick a top 3, not rate 1-5).
2. **MaxDiff lite** (which is the most important AND which is the least important).

## When to use

- You have at least 20 features to evaluate. Fewer than that, just talk to 5 customers directly.
- You have 50+ active users to send to. Below that, surveys are unreliable; do interviews.
- You're at the stage where you have *enough* features that prioritization is a real problem. Not month 1.

## When NOT to use

- You're deciding whether to build a single feature. Just ask 5 people if they'd use it (template 01).
- You're choosing between two design approaches. That's a design call. Don't crowdsource it.

## Setup

> "Quick survey, 4 minutes. We're planning the next quarter. Your answers go straight into prioritization. We can't build everything, so the ranking helps us decide."

Send to active users only. Inactive users will rank random features they'd never use.

## Template

### Question 1: Identify the user (1 question)

**Which best describes how you use [product]?**

List 3-5 personas you've defined. If you don't have personas, ask:

**What's your primary role?** (5-7 broad buckets)

You'll segment the answers by role afterward.

### Question 2: Top 3 must-have (the core question)

**Below is a list of features we're considering. Pick the THREE you'd want most. You cannot pick more than three. Picking nothing is allowed.**

Then list 10-15 features with one-sentence descriptions. Format each like:

> **Bulk export to CSV**: download all your records as a spreadsheet, including filters.

Be specific. Vague feature names ("better reporting") collect agreement for different reasons.

Use checkboxes with a hard 3-cap (most form tools support this).

### Question 3: Top 1 deal-breaker

**Of those three, which ONE would make the biggest difference to your work?**

This separates "yes nice" from "yes please".

### Question 4: Bottom 3 don't-care

**Pick the THREE features you would NOT use, even if we built them tomorrow.**

This is the question most surveys miss. People are willing to tell you what they don't want if you ask directly. Without it, every feature looks equally desirable.

### Question 5: What's missing? (open-ended, optional)

**Is there something we didn't list that would be more valuable than anything above?**

Optional. Read every answer. Some will be feature ideas, some will be complaints about existing features (which is more useful).

### Question 6: Effort context (optional)

**Knowing that bigger features take longer to build, would you rather have:**
- 3 small improvements in 3 months
- 1 large improvement in 3 months

Asking about tradeoff between small and big helps. People otherwise pick "build the biggest feature" by default and then complain when smaller fixes get deprioritized.

## Anti-patterns

| Don't | Why |
|-------|-----|
| Use a 1-5 importance scale | Everything comes back 4 or 5. Useless. |
| Allow unlimited "must have" picks | They'll pick all of them. Useless. |
| Include features you've already decided to build | You're not learning anything; you're seeking validation. |
| Hide the "I won't use this" question | This is the most informative question. Lead with it if anything. |
| Send to inactive users | Their answers are uncorrelated with usage. |
| Tell respondents the results will be shared | They'll vote strategically. Keep it private. |

## Analysis

### Compute three numbers per feature

For each feature, count:

1. **Want score**: how many respondents picked it in their top 3
2. **Reject score**: how many picked it in their "wouldn't use"
3. **Net score**: want - reject

A feature with want=40 and reject=2 is consensus.
A feature with want=40 and reject=35 is polarizing - some users need it, others actively don't want it. That's a segmentation signal, not a roadmap signal.

### Segment by persona

Re-run the same analysis filtered by Question 1 (persona). The features that win overall might lose for your most important segment.

### Compare to your gut

Before reading the results, write down what you think the top 3 will be. The features where your prediction was wrong are the ones you most needed to ask about.

## What to do with the results

The survey is input, not output. Combine with:
- Effort estimates from engineering
- Strategic fit (does this open a new segment, or just retain existing users?)
- The verbatim answers from Question 5

A feature with the highest want score is not automatically the right thing to build next. But a feature with low want and high reject is almost always the wrong thing.
