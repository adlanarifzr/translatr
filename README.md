## <a name="table-of-contents"></a>Table of Contents
* [Introduction](#introduction)
* [Installation](#installation)
* [Usage](#usage)
* [Support & Thanks](#support-&-thanks)
* [License]($license)

# Introduction
To display a translated static text might be easy with laravel, yet to display a translated data from database/model would usually require a little bit of efforts. Translatr helps to simplify the translation concept by integrating a simple trait into the Models without having to have extra tables and such.

## Installation
1. Simply put the ```Translatr.php``` into App/Traits
2. Use the Trait in your Model 
```php
use App\Traits\Translatr;

class ModelName extends Model
{
    use Translatr;
}
```

## Usage
You can display any translated data in your database by adding column name with ```_locale``` at the end of the column/attribute name. For example ```description_en``` for English and ```description_my``` for Malay language.
```php
echo $model->description;
```
This command will display the description based on your current locale.

## Support & Thanks
I would be really grateful if you would contribute to support my contributions in Laravel development by saying thanks to [adlanarifzr@gmail.com](mailto:adlanarifzr@gmail.com).

## License
The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
