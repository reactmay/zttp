# Zttp

Zttp is a simple Guzzle wrapper designed to provide a really pleasant development experience for most common use cases.

If you need more functionality, just use [Guzzle](https://github.com/guzzle/guzzle) :)

Real documentation is in the works, but for now [read the tests](https://github.com/reactmay/zttp/blob/master/tests/ZttpTest.php).

```php
$response = Zttp::withHeaders(['Fancy' => 'Pants'])->post($url, [
    'foo' => 'bar',
    'baz' => 'qux',
]);

$response->status();
// int

$response->isOk();
// true / false

$response->json();
// => [
//  'whatever' => 'was returned',
// ];
```

## Installation

`composer require reactmay/zttp`
