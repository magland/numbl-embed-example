<script src="https://numbl.org/numbl-embed.js"></script>

This demonstrates how to embed numbl in a markdown file that can be rendered on GitHub Pages.

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

disp('Sum of diagonal:')
disp(sum(diag(A)))

disp('Total sum:')
disp(sum(sum(A)))
</script>
</numbl-embed>

If it worked, you should see an embedded numbl above with a matrix operations example.

Here's a plotting example:

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

Here's an interactive REPL where you can type and run commands:

<numbl-embed mode="repl">
<iframe width="100%" height="500" frameborder="0"></iframe>
</numbl-embed>
