# eluquent-sluggable-Arabic

How to use arabic languages in Laravel [Eloquent Sluggable](https://github.com/cviebrock/eloquent-sluggable)

 [Eloquent Sluggable](https://github.com/cviebrock/eloquent-sluggable) كيف تستعمل اللغة العربية في مكتبة

##installation 


1. Go to Slugify.php file in Dir :

    
2. Change the const `LOWERCASE_NUMBERS_DASHES` to :


3. Replace `vendor/cocur/slugify/src/RuleProvider/DefaultRuleProvider.php` with [DefaultRuleProvider](https://github.com/nodekits/eluquent-sluggable-arabic/blob/master/DefaultRuleProvider.php)


##طريقة العمل

- توجه الى الملف Slugify.php  في المجلد التالي : 

    /vendor/cocur/slugify/src/Slugify.php
    
- غير القيمة الثابتة `LOWERCASE_NUMBERS_DASHES` الى 
  
 ```php
const LOWERCASE_NUMBERS_DASHES = '/([^\p{Arabic}a-zA-Z0-9]+|-+)/u';  
```

- توجه الى الملف [DefaultRuleProvider](https://github.com/nodekits/eluquent-sluggable-arabic/blob/master/DefaultRuleProvider.php) ثم استبدله بالملف التالي : 


Thx for [Abanoub Samaan](https://github.com/abanoubsamaan)
