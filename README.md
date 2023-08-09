![tests](https://github.com/jeyroik/df-templates-triggers/workflows/PHP%20Composer/badge.svg?branch=master&event=push)
![codecov.io](https://codecov.io/gh/jeyroik/df-templates-triggers/coverage.svg?branch=master)

[![Latest Stable Version](https://poser.pugx.org/jeyroik/df-templates-triggers/v)](//packagist.org/packages/jeyroik/df-templates-triggers)
[![Total Downloads](https://poser.pugx.org/jeyroik/df-templates-triggers/downloads)](//packagist.org/packages/jeyroik/df-templates-triggers)
[![Dependents](https://poser.pugx.org/jeyroik/df-template-triggerss/dependents)](//packagist.org/packages/jeyroik/df-templates-triggers)


# df-templates-triggers

Templates for DF triggers

Library provide `IContextTrigger`.

# usage

```php
$ts = new TemplateService();
$templates = $ts->getTemplates($someRepo, new ContextTrigger([
    ContextTrigger::FIELD__PARAMS => [
        ContextTrigger::PARAM__FOR => [
            IParam::FIELD__NAME => ContextTrigger::PARAM__FOR,
            IParam::FIELD__VALUE => ETrigger::Event
        ],
        ContextTrigger::PARAM__TRIGGER => [
            IParam::FIELD__NAME => ContextTrigger::PARAM__TRIGGER,
            IParam::FIELD__VALUE => $trigger
        ]
    ]
]));
```