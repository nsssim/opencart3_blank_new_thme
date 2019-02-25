# opencart 3 blank new theme :
This is my OpenCart theme skeleton that helps me creating new themes quickly
Just download and upload it to your server and activate the bilisimguru theme, find below, instruction on how to change the theme name to your liking 

### Note

keep in min that below, `bilisimguru` will be our theme name, feel free to change it to any name of your choice !


### step 1

|copy| to|
|------| ------|
|catalog/view/theme/default| catalog/view/theme/bilisimguru |

then edit 

> catalog/view/theme/bilisimguru/template/common/header.twing

```sh
//line 25 : change ref for the css from "default" to "bilisimguru"
```
### step 2
|copy| to|
|------| ------|
|admin/language/en-gb/extension/theme/default.php | admin/language/en-gb/extension/theme/bilisimguru.php |

then edit 

> admin/language/en-gb/extension/theme/bilisimguru.php

```sh

{
 $_['heading_title'] = "bilisimguru Web Theme" ; 
} 

```

### step 3
|copy| to|
|------| ------|
|admin/view/template/extension/theme/default.twig| admin/view/template/extension/theme/bilisimguru.twig|

then edit

> admin/view/template/extension/theme/bilisimguru.twig

```sh
search and replace "theme_default" to "theme_bilisimguru"
```

###  step 4
|copy| to|
|------| ------|
|admin/controller/extension/theme/default.php| admin/controller/extension/theme/bilisimguru.php|

then edit

> admin/controller/extension/theme/bilisimguru.php

```sh
{
	change : $this->load->language('extension/theme/default'); 
	to : $this->load->language('extension/theme/bilisimguru'); 
	
	search and replace "theme_default" to "theme_bilisimguru"
	//192 occurences
	
	search and replace "default" to "bilisimguru" one by one 
	
	change Class name from ControllerExtensonThemeDefault to ControllerExtensonThemeBilisimguru
	
}
```

### step 5

log in your back store and go to 

> admin===> extension > themes

> action [+] to install

> edit => status enabled 

> save


###  step 6

change theme under system settings store 

### step 7

Enjoy your new theme and Start coding :) 













