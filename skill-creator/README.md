# skill-creator

A skill for creating, improving, and evaluating other skills through iterative testing and benchmarking.

## Source

This skill was originally created by **Anthropic** as part of the [anthropics/skills](https://github.com/anthropics/skills/tree/main/skills/skill-creator) repository.

- **Original Location:** https://github.com/anthropics/skills/tree/main/skills/skill-creator
- **License:** See the original repository for licensing terms

## What It Does

This skill enables a systematic approach to skill development:

1. **Capture Intent** - Understand what the skill should do and when to trigger
2. **Draft Skills** - Write SKILL.md with proper structure and progressive disclosure
3. **Test Cases** - Create realistic test prompts and run evaluations
4. **Benchmark** - Compare with-skill vs baseline runs with quantitative metrics
5. **Iterate** - Improve based on user feedback and quantitative results
6. **Description Optimization** - Optimize triggering accuracy via eval queries

## The Core Loop

```
1. Figure out what the skill is about
2. Draft or edit the skill
3. Run claude-with-access-to-the-skill on test prompts
4. With the user, evaluate the outputs:
   - Create benchmark.json and run generate_review.py
   - Run quantitative evals
5. Repeat until satisfied
6. Package the final skill
```

## When to Use

- Creating a new skill from scratch
- Updating or optimizing an existing skill
- Running evals to test skill performance
- Benchmarking skill performance with variance analysis
- Optimizing a skill's description for better triggering accuracy

## Key Features

- **Progressive Disclosure** - Three-level loading system for efficient context usage
- **Parallel Evaluation** - Spawn with-skill and baseline runs simultaneously
- **Quantitative Assertions** - Objectively verifiable metrics for skill performance
- **HTML Reviewer** - Browser-based interface for qualitative feedback
- **Description Optimizer** - Automated loop for improving trigger accuracy
