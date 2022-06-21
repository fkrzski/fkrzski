```php
<?php

namespace fkrzski;

class Me extends Programmer
{
    public function getInformation(): array
    {
        return [
            'name' => 'Filip',
            'surname' => 'Krzyżanowski',
            'age' => 20
        ];
    }

    public function getKnowledge(): array
    {
        return [
            Php::class,
            Laravel::class,
            TestDrivenDevelopment::class,
            ModelViewController::class,
            MySQL::class,
            Git::class,
            JavaScript::class,
            Python::class,
            Css::class,
            Scss::class,
            Bootstrap::class,
        ];
    }

    public function getProjects(): array
    {
        return [
            'DeadByStats' => 'https://deadbystats.eu',
            'Dotenv' => 'https://github.com/fkrzski/Dotenv'
        ];
    }
}

$me = new Me();

foreach ($me->getProjectsAndSites() as $name => $link) { 
    echo $name.': '.$link.'<br>';
}

// Output:
```
DeadByStats: https://deadbystats.eu <br>
Dotenv: https://github.com/fkrzski/Dotenv
<!---
fkrzski/fkrzski is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
