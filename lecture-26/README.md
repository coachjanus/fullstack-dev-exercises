# fullstack-dev-exercises

## Exercises for lecture #26 inherits

- Переписати кожний з контролерів HomeController.php, AboutController.php, ContactController.php, ErrorController.php, розширюючи їх від базового класу BaseController:

```php

<?php declare(strict_types=1);

namespace Core\Http;

use Core\Kernel;
use Core\Renderer\View;

class BaseController
{
    private View $view;
    protected string $layout;

    public function __construct() 
    {
        $templates = Kernel::projectDir()."/views";
        $this->view = new View(path: $templates, layout: $this->layout);
    }
    protected function view(): View
    {
        return $this->view;
    }
}

```

- Виконайте push проекту php.dev на власний віддалений git-репозиторій 
