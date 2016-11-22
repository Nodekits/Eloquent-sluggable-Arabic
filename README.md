# eluquent-sluggable-Arabic | Slugify-Arabic

How to use arabic languages in Laravel [Eloquent Sluggable](https://github.com/cviebrock/eloquent-sluggable) & [Slugify](https://github.com/cocur/slugify)

[Eloquent Sluggable](https://github.com/cviebrock/eloquent-sluggable) & [Slugify](https://github.com/cocur/slugify) كيف تستعمل اللغة العربية في مكتبة

##installation 

1. Go to Slugify.php file in Dir :

 ```
/vendor/cocur/slugify/src/Slugify.php
```
    
2. Change the const `LOWERCASE_NUMBERS_DASHES` to :

 ```php
const LOWERCASE_NUMBERS_DASHES = '/([^\p{Arabic}a-zA-Z0-9]+|-+)/u';  
```

3. Replace `vendor/cocur/slugify/src/RuleProvider/DefaultRuleProvider.php` with [DefaultRuleProvider](https://github.com/nodekits/eluquent-sluggable-arabic/blob/master/DefaultRuleProvider.php)


##طريقة العمل

1. توجه الى الملف Slugify.php  في المجلد التالي : 
 ```
/vendor/cocur/slugify/src/Slugify.php
```
    
2. غير القيمة الثابتة `LOWERCASE_NUMBERS_DASHES` الى 
  
 ```php
const LOWERCASE_NUMBERS_DASHES = '/([^\p{Arabic}a-zA-Z0-9]+|-+)/u';  
```

3. توجه الى الملف [DefaultRuleProvider](https://github.com/nodekits/eluquent-sluggable-arabic/blob/master/DefaultRuleProvider.php) ثم استبدله بالملف التالي : 


Thx for [Abanoub Samaan](https://github.com/abanoubsamaan)
