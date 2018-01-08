## <a name="table-of-contents"></a>Table of Contents
* [Introduction](#introduction)
* [Installation](#installation)
* [Usage](#usage)
* [Support & Thanks](#support)
* [License]($license)

# Introduction
To display a translated static text might be easy with Laravel, yet to display a translated data from database/model would usually require a little bit of efforts and lines of code. Translatr helps to simplify the translation concept by integrating a simple trait into the Models without having to have extra tables and such.

## Installation
1. Install the package through composer
```
composer require adlanarifzr/translatr
```
2. Use the Translatr in your Model 
```php
use Translatr\Translatr;

class ModelName extends Model
{
    use Translatr;
}
```

## Usage
You can translate any data in your database by adding column name with ```_locale``` at the end of the column/attribute name. For example ```description_en``` for English and ```description_my``` for Malay language.
```php
echo $model->description;
```
This command will display the description based on your current locale. To add more language, simply add new column with different locale.

## <a name="support"></a>Support & Thanks
I would be really grateful if you would contribute to support my development in Laravel packages. I can be reached at [adlanarifzr@gmail.com](mailto:adlanarifzr@gmail.com).

## License
The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
