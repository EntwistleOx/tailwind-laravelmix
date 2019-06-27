# tailwind-laravelmix


$| npm install
$| npm run dev
$| npm install tailwindcss --save-dev
$| npx tailwind init

C:\laragon\www\birdboard\resources\sass\app.scss
	+|	@tailwind base;
	+|	@tailwind components;
	+|	@tailwind utilities;

$| npm install laravel-mix-tailwind --save-dev

C:\laragon\www\birdboard\webpack.mix.js
	+| let mix = require('laravel-mix');
	+| require('laravel-mix-tailwind');
	+| mix
    +|	.js('resources/js/app.js', 'public/js')
    +|	.less('resources/less/app.less', 'public/css')
    +|	.tailwind('tailwind.config.js');

$| npm run dev
