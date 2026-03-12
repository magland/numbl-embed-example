> **Early Stage & Experimental** - This project is in early development and should be considered experimental.

# numbl Embed Example

This repository demonstrates how to embed interactive MATLAB scripts in Markdown files using [numbl-embed](https://github.com/flatironinstitute/numbl). When rendered on GitHub Pages, the embedded scripts become editable and executable directly in the browser via [numbl](https://numbl.org).

## Example

* **Rendered**: [example1](https://magland.github.io/numbl-embed-example/example1)
* **Source**: [example1.md](https://raw.githubusercontent.com/magland/numbl-embed-example/refs/heads/main/example1.md)

```markdown
<script src="https://numbl.org/numbl-embed.js"></script>

This demonstrates how to embed numbl in a markdown file that can be rendered on GitHub pages.

<numbl-embed>
<iframe width="100%" height="600" frameborder="0"></iframe>
<script type="text/plain" class="matlab-script">
% Matrix operations example
A = [8, 1, 6; 3, 5, 7; 4, 9, 2];
disp('Matrix A:')
disp(A)

disp('Sum of each row:')
disp(sum(A, 2))

disp('Sum of each column:')
disp(sum(A, 1))
</script>
</numbl-embed>
```

It even works with plotting:

```markdown
<script src="https://numbl.org/numbl-embed.js"></script>

This demonstrates how to embed numbl in a markdown file that can be rendered on GitHub pages.

<numbl-embed>
<iframe width="100%" height="600" frameborder="0"></iframe>
<script type="text/plain" class="matlab-script">
% Damped oscillation
t = linspace(0, 10, 200);
y = exp(-0.3 * t) .* sin(2 * pi * t);
plot(t, y)
title('Damped Oscillation')
xlabel('Time')
ylabel('Amplitude')
</script>
</numbl-embed>
```
