# Tailwind Laravelmix

Tailwind installation:

```
$| npm install tailwindcss --save-dev

```

Create Tailwind config file:

```
$| npx tailwind init
```

Add Tailwind directives to the css entry file:

```
C:\projectRoute\yourProject\resources\sass\app.scss

	+|	@tailwind base;
	+|	@tailwind components;
	+|	@tailwind utilities;
```

Install 'Laravel Mix Tailwind' extension:

```
$| npm install laravel-mix-tailwind --save-dev
```

Add extension in Mix configuration:

```
C:\projectRoute\yourProject\webpack.mix.js

	+| let mix = require('laravel-mix');
	+| require('laravel-mix-tailwind');
```

Enable the extension by calling tailwind() in the Mix chain:

```
C:\projectRoute\yourProject\webpack.mix.js

mix.js('resources/js/app.js', 'public/js')
    .sass('resources/sass/app.scss', 'public/css')
    .tailwind('tailwind.config.js');
```

That's all, compile everything down with:

```
$| npm run dev
```
