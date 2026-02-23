## Patterns

The Generative AI will understand bracket patterns like [color] or [shape] as placeholders, and they will not affect the response as long as you replace them before sending the prompt.

If you don’t replace them, the model will usually treat them as literal text or try to guess what you mean.

## Recommended Pattern Style

Use one of the following conventions consistently All three work. The AI does not care — consistency is what matters.

### Square Brackets

Good for personal templates.

```css
Tell me the [color] of the ball.

```

### Curly Braces

Often clearer for variables.

```css
Tell me the {color} of the ball.
```

### Double Angle Brackets

Very explicit placeholders.

```sql
Tell me the <<color>> of the ball.
```

## What Happens If You Don’t Replace Patterns?

Possible outcomes:

* The model might answer: “The color of the ball is not specified.”

* Or it may interpret `[color]` as a literal word.

* Rarely, it may guess randomly.

So it won’t “break”, but it won’t behave like a variable system either.

## Best Practice for an .md Prompt Pattern File

Store templates like this:

```md
# Prompt Patterns

## Object Description

Tell me the {attribute} of the {object}.

Example:  
Tell me the color of the ball.  
Tell me the shape of the ball.

```

This keeps:

* Pattern reusable

* Default untouched

* Examples visible

* Copy-paste friendly

## Contributions

Contributions and feedback are welcome! If you have suggestions for improvements or additional tools, feel free to open an issue or submit a pull request.

## License

This project is licensed under the [CC0 1.0 Universal](LICENSE) - see the [LICENSE](LICENSE) file for details.
