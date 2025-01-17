#下雪代码css
```css
.index-one{
    height: 70vh;
    width: 100vw;
    position: relative;
    background: black;
    overflow: hidden;
    margin: 0;
	padding: 0;
	background: url("https://hagall-media.de/cp/forest3.jpg") repeat-x;
	background-position: center bottom;
	background-size: cover;
}

canvas {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
}

#snow-canvas-1 {
	z-index: 6;
}
#snow-canvas-2 {
	z-index: 5;
}
#snow-canvas-3 {
	z-index: 4;
}
#snow-canvas-4 {
	z-index: 3;
}
#snow-canvas-5 {
	z-index: 2;
}
#snow-canvas-6 {
	z-index: 1;
}

.clouds-bg {
	height: 70vh;
    width: 100vw;
	z-index: 0;
	position: relative;
	background: url("https://hagall-media.de/cp/clouds.png") repeat-x;
	background-size: cover;
	animation: moveClouds 200s linear infinite;
}

@keyframes moveClouds {
	0% {
		background-position: 0 0;
	}
	100% {
		background-position: -2000px 0;
	}
}
```

# prism.min.js
代码块使用:

下载prism.min.js 引用

```html
<?php if ($this->options->PrismTheme) : ?>
<link href="<?php $this->options->PrismTheme() ?>" rel="stylesheet">
<?php else : ?>
<link href="//npm.elemecdn.com/prismjs@1.29.0/themes/prism.min.css" rel="stylesheet">
<?php endif; ?>
```

主题设置添加

```php
$PrismTheme = new Typecho_Widget_Helper_Form_Element_Select(
    'PrismTheme',
    array(
      '//npm.elemecdn.com/prismjs@1.29.0/themes/prism.min.css' => 'prism（默认）',
      '//npm.elemecdn.com/prismjs@1.29.0/themes/prism-dark.min.css' => 'prism-dark',
      '//npm.elemecdn.com/prismjs@1.29.0/themes/prism-okaidia.min.css' => 'prism-okaidia',
      '//npm.elemecdn.com/prismjs@1.29.0/themes/prism-solarizedlight.min.css' => 'prism-solarizedlight',
      '//npm.elemecdn.com/prismjs@1.29.0/themes/prism-tomorrow.min.css' => 'prism-tomorrow',
      '//npm.elemecdn.com/prismjs@1.29.0/themes/prism-twilight.min.css' => 'prism-twilight',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-a11y-dark.min.css' => 'prism-a11y-dark',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-atom-dark.min.css' => 'prism-atom-dark',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-base16-ateliersulphurpool.light.min.css' => 'prism-base16-ateliersulphurpool.light',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-cb.min.css' => 'prism-cb',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-coldark-cold.min.css' => 'prism-coldark-cold',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-coldark-dark.min.css' => 'prism-coldark-dark',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-darcula.min.css' => 'prism-darcula',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-dracula.min.css' => 'prism-dracula',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-duotone-dark.min.css' => 'prism-duotone-dark',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-duotone-earth.min.css' => 'prism-duotone-earth',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-duotone-forest.min.css' => 'prism-duotone-forest',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-duotone-light.min.css' => 'prism-duotone-light',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-duotone-sea.min.css' => 'prism-duotone-sea',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-duotone-space.min.css' => 'prism-duotone-space',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-ghcolors.min.css' => 'prism-ghcolors',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-gruvbox-dark.min.css' => 'prism-gruvbox-dark',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-hopscotch.min.css' => 'prism-hopscotch',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-lucario.min.css' => 'prism-lucario',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-material-dark.min.css' => 'prism-material-dark',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-material-light.min.css' => 'prism-material-light',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-material-oceanic.min.css' => 'prism-material-oceanic',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-night-owl.min.css' => 'prism-night-owl',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-nord.min.css' => 'prism-nord',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-pojoaque.min.css' => 'prism-pojoaque',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-shades-of-purple.min.css' => 'prism-shades-of-purple',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-synthwave84.min.css' => 'prism-synthwave84',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-vs.min.css' => 'prism-vs',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-vsc-dark-plus.min.css' => 'prism-vsc-dark-plus',
      '//npm.elemecdn.com/prism-themes@1.9.0/themes/prism-xonokai.min.css' => 'prism-xonokai',
      '//npm.elemecdn.com/prism-theme-one-light-dark@1.0.4/prism-onelight.min.css' => 'prism-onelight',
      '//npm.elemecdn.com/prism-theme-one-light-dark@1.0.4/prism-onedark.min.css' => 'prism-onedark',
      '//npm.elemecdn.com/prism-theme-one-dark@1.0.0/prism-onedark.min.css' => 'prism-onedark2',
    ),
    '//npm.elemecdn.com/prismjs@1.29.0/themes/prism.min.css',
    '选择一款您喜欢的代码高亮样式',
    '介绍：用于修改代码块的高亮风格 <br>
         其他：如果您有其他样式，可通过源代码修改此项，引入您的自定义样式链接'
  );
  $form->addInput($PrismTheme);
```
