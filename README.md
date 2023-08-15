```php
<?php

namespace fkrzski;

class Me extends Developer
{
    public function getInformation(): array {
        return [
            'name' => 'Filip',
            'surname' => 'Krzyżanowski',
            'age' => 21
        ];
    }

    public function getKnowledge(): array {
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

    public function getProjects(): array {
        return [
            'DeadByStats' => 'https://deadbystats.eu',
            'Dotenv' => 'https://github.com/fkrzski/Dotenv',
            'RynekGPU' => 'https://rynekgpu.dmisiek.pl/'
        ];
    }
}

foreach ((new Me())->getProjects() as $name => $link) {
    echo $name.': '.$link.'<br>';
}

// Output:
```

DeadByStats: https://deadbystats.eu <br>
Dotenv: https://github.com/fkrzski/Dotenv <br>
RynekGPU: https://rynekgpu.dmisiek.pl

