# 08. Pricing research

## Goal

You're setting a price for the first time, or you're considering a change. You want signal that's better than "what feels right".

The most-asked pricing question - "What would you pay for this?" - is also the worst. People give a number to be polite, not a number they'd actually pay. This template avoids it.

## Three techniques, choose the right one

| Technique | Use when |
|-----------|----------|
| **Van Westendorp** | Pre-launch. You have no users yet. You need a rough range, not a precise number. |
| **Conjoint-style tradeoff** | You have a few competing plan structures and want to know which mix wins. |
| **Willingness-to-pay anchored to alternatives** | You have users and competitors. You want to position your price among existing options. |

Don't try to do all three in one survey.

## Technique 1: Van Westendorp price sensitivity

Four questions, asked in this exact order:

1. At what price would you consider [product] to be **too expensive** to consider buying?
2. At what price would you consider it **so expensive** you'd question its value?
3. At what price would you consider it to be a **bargain** - great value for money?
4. At what price would you consider it to be **so cheap** you'd doubt the quality?

Notes:
- Numeric input only. Allow a "would not buy at any price" option.
- Describe the product clearly *before* asking. Vague descriptions produce vague numbers.
- Use a currency input with a hard floor at 0.

When you have 100+ responses, plot:
- Cumulative percent who said "too expensive" at price X (rises with X)
- Cumulative percent who said "bargain" at price X (falls with X)
- Cumulative "so expensive" and "so cheap"

The crossover points give you:
- Lower acceptable bound: where "too cheap" meets "bargain"
- Optimal price point: where "too expensive" meets "too cheap"
- Upper acceptable bound: where "too expensive" meets "bargain"

These are ranges, not exact numbers. Treat them as the band inside which you make a judgment call.

## Technique 2: Conjoint-style tradeoff

You have three plan structures in mind. Don't ask which they prefer. Ask them to make tradeoffs.

Present three plans:

> **Plan A**: $49/month, includes [feature set 1]
> **Plan B**: $99/month, includes [feature set 1 + 2]
> **Plan C**: $199/month, includes [feature set 1 + 2 + 3]

Then ask:

1. Which would you pick today, given your current needs?
2. Which would you NOT pick under any reasonable scenario?
3. What's missing from your pick that makes you hesitate?
4. What's included in your pick that you don't need?

The "what's included you don't need" question is the most informative. People can articulate the waste in someone else's pricing better than they can articulate the value in their own.

Iterate the plans 2-3 times based on responses before finalizing. The first pass is rarely right.

## Technique 3: Willingness-to-pay anchored to alternatives

You have 50+ existing users or a clear competitive landscape. Ask:

1. Are you currently paying for any tool that overlaps with what [product] does? Which one(s)?
2. About how much, per month?
3. Compared to [competitor], how would you describe [our product]? Better in some ways and worse in others, much better overall, about the same, or worse?
4. If [our product] cost the same as [competitor], would you switch?
5. If [our product] cost 50% more, would you still switch? Why?

This is more honest than asking "what would you pay". You're triangulating on price by anchoring to a real existing decision.

## Anti-patterns

| Don't | Why |
|-------|-----|
| Ask "What's a fair price for [product]?" | They have no idea. Their number is a polite guess. |
| Ask "Would you pay $X/month?" | Yes/no with one number is too coarse. They might pay 5 dollars more or 50 dollars less. |
| Offer a discount during the research | You're now researching discount-seeking behavior, not real price sensitivity. |
| Show your pricing page mid-survey | Anchors them to your existing prices. You learn nothing. |
| Trust the answers from people who haven't actually bought a similar tool | Their numbers are imagination. Weight responses by whether they've paid for *something* in the category. |

## After research: judgment

Pricing research gives you a range. The exact number inside that range is a strategic call:

- **Lower end of the range**: optimize for adoption and word-of-mouth. Make sense if your product has network effects or you're trying to commoditize a competitor.
- **Upper end of the range**: optimize for revenue per customer. Makes sense if your costs scale with usage, or if you're targeting a small high-value segment.
- **Above the upper end**: only if you have positioning that supports it (enterprise, regulated, lock-in).
- **Below the lower end**: usually a mistake. Race-to-the-bottom rarely works for software.

The research narrows the band. Strategy picks the point inside the band.

## What this template won't do

It won't tell you:
- Whether to charge per-seat, per-usage, flat-rate, or tiered (that's a positioning and unit-economics question)
- Whether to offer a free tier (depends on activation funnel, not on willingness-to-pay)
- Whether to offer annual discounts (yes, almost always)

Those are decisions, not research outputs.
