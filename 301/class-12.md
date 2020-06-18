# EJS Partials

[EJS Partials](https://medium.com/@henslejoseph/ejs-partials-f6f102cb7433)

[EJS Tutorial Video](https://www.youtube.com/watch?v=3_xEEH4fTEk&t=0s&index=7&list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)

Partials come in handy when you want to reuse the same HTML across multiple views. Think of partials as functions, they make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in. Instead, you define that reusable bundle of code in a file and include it wherever you need it.

Note: The <%- %> tags allow us to output the unescaped content onto the page (notice the -). This is important when using the include ( ) statement since you don’t want EJS to escape your HTML characters like ‘<’, ‘>’, etc…