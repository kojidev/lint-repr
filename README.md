`php bin/console lint:container -e prod`

xdebugger at: `vendor/symfony/dependency-injection/Compiler/CheckTypeDeclarationsPass.php:202`
with condition: `$value === '%sentry.listener_priorities.console%'`
is where value gets assigned empty array, although it is a number: 

`php bin/console debug:container --parameter=sentry.listener_priorities.console` prints `1`
