# JSLog
 JavaScript library for server-side log. Simple to use, flexible and light-weight (only 3k).

## Getting Started

Use ```JSLog.js``` for debugging purposes or development environments:
```html
<script type="text/javascript" src="JSLog.js"></script>
```
Use ```JSLog.min.js``` in production:
```html
<script type="text/javascript" src="JSLog.min.js"></script>
```
Project wiki: _work in progress..._

## Call documentation

* log: POST request with JSON body
  ```json
  [
   {
     "level": "TRACE",
     "entity": 1,
     "log_key": "KEY",
     "message": "HELLO!",
     "Host": "MyHost",
     "UserAgent": "Mozilla...",
     "datetime": "2019-05-01T12:00:00",
     "httpCode": 0
   },
   ...
  ]
  ```
* profile: POST request with JSON body
  ```json
  {
    "entity": 1,
    "log_key": "KEY",
    "time": 1000,
    "desc": "request_1"
  }
  ```
  
The fields _entity_, _log_key_, _Host_, _UserAgent_, _httpCode_ are optional for both.

## Running test

Unit test: _work in progress..._

See also:
 * [PHP](https://github.com/rippetanks/PHP_example_JSLog)
 * [Java](https://github.com/rippetanks/JSLog_Java)

## Versioning

We use [SemVer](http://semver.org/) for versioning.

## Authors

* **Simone Martelli** - *Project Manager and Software developer*

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
