<div align="center">

# Awesome Swoole with stars

A curated list of awesome things related to <a href="//github.com/swoole/swoole-src">Swoole</a>.

<img width="200" height="120" align=center alt="Swoole Logo" src="https://cdn.jsdelivr.net/gh/sy-records/staticfile/images/swoole/logo.png">

</div>

# Table of Contents

* [Awesome Swoole](#awesome-swoole----)
  * [Architectural](#architectural)
  * [Client Packages](#client-packages)
  * [Cronjobs](#cronjobs)
  * [Database](#database)
  * [Debugging and Profiling](#debugging-and-profiling)
  * [Development Environment](#development-environment)
  * [Distribution](#distribution)
  * [Frameworks](#frameworks)
  * [Framework Integration](#framework-integration)
  * [gRPC](#grpc)
  * [HTTP and WebSocket](#http-and-websocket)
  * [Logging](#logging)
  * [Serverless](#serverless)
  * [SOA governance](#soa-governance)
  * [Tasks and Queues](#tasks-and-queues)
  * [Testing](#testing)
  * [Third-party SDK](#third-party-sdk)
  * [Web Applications](#web-applications)
  * [Miscellaneous](#miscellaneous)
* [Resources](#resources)
  * [Swoole Books](#swoole-books)
  * [Swoole Videos](#swoole-videos)
  * [Miscellaneous](#miscellaneous-1)

NOTE: Projects labelled with emoji :globe\_with\_meridians: have their documentation written in non-English languages.

## Architectural

*Libraries related to design patterns, programming approaches and ways to organize code.*

* [leocarmo/circuit-breaker-php](https://github.com/leocarmo/circuit-breaker-php) ⭐ 302 | 🐛 3 | 🌐 PHP | 📅 2025-07-01 - PHP implementation of Circuit Breaker Pattern.
* [Phluxor] - An implementation of the Actor model for PHP.

## Client Packages

* [simps/mqtt](https://github.com/simps/mqtt) ⭐ 398 | 🐛 0 | 🌐 PHP | 📅 2026-07-26 - A coroutine-based MQTT client. It supports MQTT version 3.1, 3.1.1, and 5.0.
* [swoole/ext-zookeeper](https://github.com/swoole/ext-zookeeper) ⭐ 152 | 🐛 1 | 🌐 C | 📅 2025-08-25 - A Swoole-based ZooKeeper client. :globe\_with\_meridians:
* ~~[swoole/ext-postgresql](https://github.com/swoole/ext-postgresql) ⚠️ Archived~~ - A Swoole-based PostgreSQL client. The repository has been archived by its owner. PostgreSQL support is now built into Swoole itself, enabled at compile time with the `--enable-swoole-pgsql` flag.
* [hyperf/jet](https://github.com/hyperf/jet) ⭐ 61 | 🐛 2 | 🌐 PHP | 📅 2024-01-11 - An RPC Client with built-in support for [the JSON-RPC protocol](https://www.jsonrpc.org/). It works with both PHP-FPM and Swoole.
* [hyperf/elasticsearch](https://github.com/hyperf/elasticsearch) ⭐ 7 | 🐛 1 | 🌐 PHP | 📅 2026-06-07 - The [Elasticsearch] client of Hyperf.
* [hyperf/etcd](https://github.com/hyperf/etcd) ⭐ 6 | 🐛 0 | 🌐 PHP | 📅 2026-06-07 - The [etcd](https://etcd.io) client of Hyperf.
* [hyperf/consul](https://github.com/hyperf/consul) ⭐ 4 | 🐛 2 | 🌐 PHP | 📅 2026-06-07 - The [Consul] client of Hyperf.

## Cronjobs

* [osgochina/swoole-crontab](https://github.com/osgochina/swoole-crontab) ⭐ 968 | 🐛 13 | 🌐 PHP | 📅 2021-01-08 - A Swoole-based crontab schedule. It allows jobs to run at intervals of seconds, and is fully compatible with crontab syntax. :globe\_with\_meridians:
* [hyperf/crontab](https://github.com/hyperf/crontab) ⭐ 13 | 🐛 6 | 🌐 PHP | 📅 2026-06-07 - The cron component of Hyperf, allowing jobs to run at intervals of seconds.

## Database

* [SMProxy](https://github.com/louislivi/SMProxy) ⭐ 1,760 | 🐛 16 | 🌐 PHP | 📅 2022-11-13 - SMProxy (Swoole MySQL Proxy), A MySQL database connection pool library. :globe\_with\_meridians:
* [open-smf/connection-pool](https://github.com/open-smf/connection-pool) ⭐ 222 | 🐛 12 | 🌐 PHP | 📅 2024-05-16 - A common connection pool based on Swoole.
* [simple-swoole/db](https://github.com/simple-swoole/db) ⭐ 20 | 🐛 4 | 🌐 PHP | 📅 2023-02-06 - The database component of [Simps](https://github.com/simple-swoole/simps) ⭐ 477 | 🐛 1 | 🌐 PHP | 📅 2022-05-30. This component is built on top of [the Swoole Library](https://github.com/swoole/library) ⭐ 251 | 🐛 1 | 🌐 PHP | 📅 2026-07-30.
* [hyperf/database](https://github.com/hyperf/database) ⭐ 19 | 🐛 3 | 🌐 PHP | 📅 2026-07-29 - The database component of Hyperf.
* [mix/database](https://github.com/mix-php/database) ⭐ 15 | 🐛 1 | 🌐 PHP | 📅 2025-11-04 - A Swoole-based database component, with built-in support for connection pool. :globe\_with\_meridians:
* [mix/redis-subscriber](https://github.com/mix-php/redis-subscriber) ⭐ 15 | 🐛 0 | 🌐 PHP | 📅 2024-06-06 - A Swoole-based Redis subscription component. :globe\_with\_meridians:
* [mix/redis](https://github.com/mix-php/redis) ⭐ 5 | 🐛 0 | 🌐 PHP | 📅 2023-04-04 - A Swoole-based Redis component, with built-in support for connection pool. :globe\_with\_meridians:

## Debugging and Profiling

* [apache/skywalking-php](https://github.com/apache/skywalking-php) ⭐ 180 | 🐛 0 | 🌐 Rust | 📅 2026-07-01 - The PHP Agent for [Apache SkyWalking](https://skywalking.apache.org), which provides native tracing and PHP Health Metrics (PHM) runtime reporting for PHP and Swoole projects.
* [swoole/debugger](https://github.com/swoole/debugger) ⭐ 77 | 🐛 0 | 🌐 PHP | 📅 2021-05-20 - A remote debugger of Swoole. By adding one-line of code, you can debug your application remotely using a rich list of commands. :globe\_with\_meridians:
* [Blackfire](https://www.blackfire.io) - A low-overhead code profiler.
  * [upscale/swoole-blackfire](https://github.com/upscalesoftware/swoole-blackfire) ⭐ 22 | 🐛 1 | 🌐 PHP | 📅 2025-02-18 - Blackfire profiler integration for Swoole web-server.
* [Xdebug](https://xdebug.org) - A debug and profile tool for PHP. Xdebug 3.1.0+ works with Swoole 5.0.2+ on PHP 8.1+ only. Lower versions of Xdebug don't work with Swoole.

## Development Environment

* Docker
  * [phpswoole/swoole](https://github.com/swoole/docker-swoole) ⭐ 565 | 🐛 1 | 🌐 Dockerfile | 📅 2026-07-27 - Official Docker image of Swoole.
  * [adhocore/lemp](https://github.com/adhocore/docker-lemp) ⭐ 164 | 🐛 5 | 🌐 Dockerfile | 📅 2024-09-09 - A single container LEMP complete fullstack with latest releases of PHP (7.4 - 8.3) and MySQL, nginx, PostgreSQL, phalcon, swoole, mailcatcher, beanstalkd, elasticsearch, memcached, redis, adminer and all you ever need.
* IDE Helper
  * [swoole/ide-helper](https://github.com/swoole/ide-helper) ⭐ 520 | 🐛 1 | 🌐 PHP | 📅 2026-07-31 - IDE help files to provide accurate autocompletion for Swoole.
  * [Swoole IDE Helper](https://plugins.jetbrains.com/plugin/13040-swoole-ide-helper) - Swoole IDE Helper for PhpStorm and Intellij IDEA. Thanks to [Luhur Abdi (Abi) Rizal](https://elabee.me) for maintaining it.

## Distribution

* [static-php-cli](https://github.com/crazywhalecc/static-php-cli) ⭐ 1,921 | 🐛 35 | 🌐 PHP | 📅 2026-08-15 - Build static PHP binary in Linux, with Swoole and other popular extensions included. :globe\_with\_meridians:
* [shivammathur/extensions](https://github.com/shivammathur/homebrew-extensions) ⭐ 821 | 🐛 1 | 🌐 Ruby | 📅 2026-08-14 - 🍻 Homebrew tap for PHP extensions.
* [swoole-cli](https://github.com/swoole/swoole-cli) ⭐ 249 | 🐛 23 | 🌐 C | 📅 2026-05-22 - A prebuilt executable to run Swoole applications directly. No PHP installation required (just download and use it). Support Linux, macOS, and Windows. :globe\_with\_meridians:

## Frameworks

* [Hyperf](https://github.com/hyperf/hyperf) ⭐ 6,884 | 🐛 444 | 🌐 PHP | 📅 2026-08-15 - A coroutine framework that focuses on hyperspeed and flexibility.
  * Official components (an incomplete list)
    * [hyperf/jet](https://github.com/hyperf/jet) ⭐ 61 | 🐛 2 | 🌐 PHP | 📅 2024-01-11
    * [hyperf/amqp](https://github.com/hyperf/amqp) ⭐ 23 | 🐛 4 | 🌐 PHP | 📅 2026-06-07
    * [hyperf/database](https://github.com/hyperf/database) ⭐ 19 | 🐛 3 | 🌐 PHP | 📅 2026-07-29
    * [hyperf/crontab](https://github.com/hyperf/crontab) ⭐ 13 | 🐛 6 | 🌐 PHP | 📅 2026-06-07
    * [hyperf/async-queue](https://github.com/hyperf/async-queue) ⭐ 9 | 🐛 2 | 🌐 PHP | 📅 2026-07-26
    * [hyperf/task](https://github.com/hyperf/task) ⭐ 9 | 🐛 1 | 🌐 PHP | 📅 2026-06-07
    * [hyperf/tracer](https://github.com/hyperf/tracer) ⭐ 9 | 🐛 2 | 🌐 PHP | 📅 2026-08-10
    * [hyperf/elasticsearch](https://github.com/hyperf/elasticsearch) ⭐ 7 | 🐛 1 | 🌐 PHP | 📅 2026-06-07
    * [hyperf/etcd](https://github.com/hyperf/etcd) ⭐ 6 | 🐛 0 | 🌐 PHP | 📅 2026-06-07
    * [hyperf/consul](https://github.com/hyperf/consul) ⭐ 4 | 🐛 2 | 🌐 PHP | 📅 2026-06-07
    * [hyperf/filesystem](https://github.com/hyperf/filesystem) ⭐ 4 | 🐛 0 | 🌐 PHP | 📅 2026-06-07
    * [hyperf/logger](https://github.com/hyperf/logger) ⭐ 4 | 🐛 0 | 🌐 PHP | 📅 2026-08-10
  * Third-party components (an incomplete list)
    * [96qbhy/hyperf-auth](https://github.com/qbhy/hyperf-auth) ⭐ 194 | 🐛 5 | 🌐 PHP | 📅 2024-01-11 - An authentication component for Hyperf. It supports JWT and session-based authentications. You can also create your own authentication drivers if needed. :globe\_with\_meridians:
    * [reasno/fastmongo](https://github.com/Reasno/fastmongo) ⭐ 89 | 🐛 17 | 🌐 PHP | 📅 2024-08-20 - A coroutine-based MongoDB client for Hyperf.
    * [opencodeco/hyperf-doctrine](https://github.com/opencodeco/hyperf-doctrine) ⭐ 4 | 🐛 0 | 🌐 PHP | 📅 2023-09-06 - This project provides an integration for the Doctrine ORM and the Hyperf framework.
    * [friendsofhyperf/components] - Some most popular third-party components for Hyperf.
* [Mix PHP](https://github.com/mix-php/mix) ⭐ 1,929 | 🐛 3 | 🌐 PHP | 📅 2026-03-18 - A unique single-threaded coroutine-based framework. :globe\_with\_meridians:
  * Official modules (an incomplete list)
    * [mix/database](https://github.com/mix-php/database) ⭐ 15 | 🐛 1 | 🌐 PHP | 📅 2025-11-04
    * [mix/redis-subscriber](https://github.com/mix-php/redis-subscriber) ⭐ 15 | 🐛 0 | 🌐 PHP | 📅 2024-06-06
    * [mix/redis](https://github.com/mix-php/redis) ⭐ 5 | 🐛 0 | 🌐 PHP | 📅 2023-04-04
    * [mix/sync-invoke](https://github.com/mix-php/sync-invoke) ⭐ 3 | 🐛 0 | 🌐 PHP | 📅 2020-10-28
    * [mix/tracing-zipkin](https://github.com/mix-php/tracing-zipkin) ⭐ 2 | 🐛 0 | 🌐 PHP | 📅 2020-09-30
    * [mix/monolog](https://github.com/mix-php/monolog) ⭐ 1 | 🐛 0 | 🌐 PHP | 📅 2020-09-30
* [imi](https://github.com/imiphp/imi) ⭐ 1,186 | 🐛 17 | 🌐 PHP | 📅 2026-07-31 - A Swoole-based framework, with built-in support for HTTP/1, HTTP/2, WebSocket, TCP, UDP, and MQTT. :globe\_with\_meridians:
* ~~[Siler](https://github.com/leocavalcante/siler) ⚠️ Archived~~ - A set of general purpose high-level abstractions aiming an API for declarative programming in PHP. The repository was archived by its owner in 2022.
* [lizhichao/one](https://github.com/lizhichao/one) ⭐ 874 | 🐛 1 | 🌐 PHP | 📅 2026-01-21 - A simple and efficient framework that works both under PHP-FPM and Swoole.
* [Ubiquity](https://github.com/phpMv/ubiquity) ⭐ 700 | 🐛 13 | 🌐 PHP | 📅 2025-11-30 - A powerful and fast framework for efficient design.
* [Simps](https://github.com/simple-swoole/simps) ⭐ 477 | 🐛 1 | 🌐 PHP | 📅 2022-05-30 - A simple, lightweight and high-performance PHP coroutine framework.
* [Nano](https://github.com/hyperf/nano) ⭐ 433 | 🐛 10 | 🌐 PHP | 📅 2023-10-08 - A Hyperf-based coroutine microframework.
* [QueryPHP](https://github.com/hunzhiwange/queryphp) ⭐ 304 | 🐛 0 | 🌐 PHP | 📅 2026-06-02 - A modern, high performance PHP progressive coroutine framework. :globe\_with\_meridians:
* ~~[Resonance](https://github.com/distantmagic/resonance) ⚠️ Archived~~ - Designed from the ground up to facilitate interoperability and messaging between services in your infrastructure and beyond. The repository was archived by its owner in 2026.
  * Official documentation: <https://resonance.distantmagic.com/>
* ~~[Fomo](https://github.com/fomo-framework/fomo) ⚠️ Archived~~ - A simple, fast framework with many features for the HTTP. It was ranked as the fastest PHP framework in the world since 2022-10-16 (and still is as of 2022-11-30) by the [Web Frameworks Benchmark](https://web-frameworks-benchmark.netlify.app/result?l=php) project. The repository was archived by its owner in 2025.
* [chubbyphp-framework](https://github.com/chubbyphp/chubbyphp-framework) ⭐ 137 | 🐛 0 | 🌐 PHP | 📅 2026-07-05: A minimal middleware based micro framework using PSR, with the goal is to achive the best combination of flexibility and simplicity by using standards.
* [Polyel](https://github.com/Superbition/Polyel-Framework) ⭐ 21 | 🐛 0 | 🌐 PHP | 📅 2022-02-14 - A full-stack MVC PHP framework/server built from the ground up based on Swoole.
* [Hypervel](https://hypervel.org) - A Laravel-style framework with native coroutine support for high performance, built on top of Swoole.
* [LightMVC](https://lightmvcframework.net) - A modular, event-driven and Swoole-enabled framework that allows to easily create PHP applications by using any PHP library.
* Laminas/Mezzio/Zend Framework
  * [mezzio/mezzio-swoole](https://github.com/mezzio/mezzio-swoole) ⭐ 93 | 🐛 16 | 🌐 PHP | 📅 2026-08-11 - Provides the support of Swoole into a [Mezzio](https://docs.mezzio.dev/) application.

## Framework Integration

*To run PHP/PHP-FPM frameworks using Swoole.*

* [PHP Runtimes](https://github.com/php-runtime/runtime) ⭐ 442 | 🐛 26 | 🌐 PHP | 📅 2025-12-18 - A home for runtimes, where people can easily create a `Runtime` to run an application with Bref, Swoole or ReactPHP without making any change to the application itself.
* Drupal
  * [The Swoole module for Drupal](https://www.drupal.org/project/swoole) - The Swoole module for Drupal supercharges your website's performance by serving it via the Swoole or the OpenSwoole PHP server. The (Open)Swoole PHP server boots Drupal once, keeps it in memory and then feeds it requests at supersonic speeds. Thanks to [daffie](https://www.drupal.org/u/daffie).
* Laravel
  * [Laravel Octane](https://github.com/laravel/octane) ⭐ 4,034 | 🐛 21 | 🌐 PHP | 📅 2026-08-13 - A first-party Laravel package that supercharges laravelish application's performance by serving it using Swoole high-performance HTTP servers. Developed and maintained by the Laravel team.
  * ~~[swooletw/laravel-swoole](https://github.com/swooletw/laravel-swoole) ⚠️ Archived~~ - A high-performance HTTP server to run Laravel/Lumen application on top of Swoole. The repository was archived by its owner in 2025. Its authors recommend *Laravel Octane* instead, or *Hypervel* if you need coroutine support.
  * [hhxsv5/laravel-s](https://github.com/hhxsv5/laravel-s) ⭐ 3,880 | 🐛 70 | 🌐 PHP | 📅 2026-07-20 - An out-of-the-box adapter between Laravel/Lumen and Swoole.
  * ~~[scil/laravel-fly](https://github.com/scil/LaravelFly) ⚠️ Archived~~ - To be an absolutely safe solution to speed up Laravel with Swoole. Preloading + Coroutine and Tinker Online. The repository was archived by its owner in 2024. Please use *Laravel Octane* instead.
  * [huang-yi/shadowfax](https://github.com/huang-yi/shadowfax) ⭐ 349 | 🐛 12 | 🌐 PHP | 📅 2022-01-15 - Runs your Laravel application on Swoole.
  * [toxmc/fast-laravel](https://github.com/toxmc/fast-laravel) ⭐ 34 | 🐛 0 | 🌐 PHP | 📅 2021-05-17 - A Swoole-based high-performance HTTP server to speed up your Laravel applications. :globe\_with\_meridians:
* Phalcon
  * [phwoolcon/phwoolcon](https://github.com/phwoolcon/phwoolcon) ⭐ 170 | 🐛 0 | 🌐 PHP | 📅 2019-07-24 - Phalcon + Swoole.
* Slim
  * ~~[pachico/Slim-Swoole](https://github.com/pachico/slim-swoole) ⚠️ Archived~~ - A convenient library to run [SlimPHP](https://www.slimframework.com) applications with Swoole. The repository was archived by its owner in 2023, and no direct replacement is known.
* Symfony
  * [symfony/runtime](https://github.com/symfony/runtime) ⭐ 740 | 🐛 0 | 🌐 PHP | 📅 2026-08-10 - The Runtime component decouples the bootstrapping logic from any global state to make sure the application can run with runtimes like PHP-FPM, ReactPHP, Swoole, etc. without any changes. For a more generic implementation that works with other frameworks/environments, please check project [PHP Runtimes](https://github.com/php-runtime/runtime) ⭐ 442 | 🐛 26 | 🌐 PHP | 📅 2025-12-18.
  * [swoole-bundle/swoole-bundle] - Symfony integration with Swoole or Open Swoole to speed up your applications.
* ThinkPHP
  * [topthink/think-swoole](https://github.com/top-think/think-swoole) ⭐ 478 | 🐛 15 | 🌐 PHP | 📅 2026-07-21 - To run ThinkPHP applications with Swoole. :globe\_with\_meridians:
* Yii
  * [liufee/yii2-swoole](https://github.com/liufee/yii2-swoole) ⭐ 341 | 🐛 1 | 🌐 PHP | 📅 2021-11-09 - To run [Yii 2](https://www.yiiframework.com) applications with Swoole. :globe\_with\_meridians:
  * [klsoft/yii3-swoole](https://github.com/klsoft-web/yii3-swoole) ⭐ 0 | 🐛 0 | 🌐 PHP | 📅 2026-08-05 - The package provides the Swoole HTTP server for the [Yii 3](https://yii3.yiiframework.com) application.
* [Utopia] - A PHP MVC based framework with minimal must-have features for professional, simple, advanced and secure web development. The Swoole server adapter ships with *Utopia* itself.
* WordPress
  * [WordPress Swoole](https://github.com/WordPress-PSR/swoole) ⭐ 87 | 🐛 5 | 🌐 PHP | 📅 2026-05-20 - To run WordPress in Swoole.

## gRPC

* [swoole/grpc](https://github.com/swoole/grpc) ⭐ 197 | 🐛 13 | 🌐 PHP | 📅 2022-09-26 - An efficient Swoole-based gRPC client. :globe\_with\_meridians:
* [mix/grpc](https://github.com/mix-php/grpc) ⭐ 58 | 🐛 2 | 🌐 PHP | 📅 2026-03-18 - A gRPC implementation based on Swoole. Protoc code generator, server, client, and more features included. :globe\_with\_meridians:
* [hyperf/grpc-client](https://github.com/hyperf/grpc-client) ⭐ 4 | 🐛 2 | 🌐 PHP | 📅 2026-08-04 - The gRPC client component of Hyperf.
* [hyperf/grpc-server](https://github.com/hyperf/grpc-server) ⭐ 3 | 🐛 0 | 🌐 PHP | 📅 2026-06-07 - The gRPC server component of Hyperf.

## HTTP and WebSocket

*Libraries for working with HTTP and WebSocket.*

* [Saber](https://github.com/swlib/saber) ⭐ 972 | 🐛 32 | 🌐 PHP | 📅 2021-10-15 - A coroutine-based HTTP client. :globe\_with\_meridians:
* [Yurunsoft/YurunHttp](https://github.com/Yurunsoft/YurunHttp) ⭐ 259 | 🐛 0 | 🌐 PHP | 📅 2026-07-24 - An easy-to-use HTTP client that works with HTTP/1, HTTP/2, and WebSocket protocols. It also supports chained operations, concurrent processing, and connection pool. :globe\_with\_meridians:
* [Yurunsoft/Guzzle-Swoole](https://github.com/Yurunsoft/Guzzle-Swoole) ⭐ 161 | 🐛 2 | 🌐 PHP | 📅 2022-01-10 - Make the [Guzzle](https://github.com/guzzle/guzzle) ⭐ 23,462 | 🐛 2 | 🌐 PHP | 📅 2026-08-09 library coroutine-friendly in Swoole. It works with many Guzzle-based packages and Swoole-based frameworks. :globe\_with\_meridians:
* [Utopia WebSocket](https://github.com/utopia-php/websocket) ⭐ 12 | 🐛 1 | 🌐 PHP | 📅 2026-05-14 - A simple and lite abstraction layer around a WebSocket server. This library is aiming to be as simple and easy to learn and use.
* PSR Compliance
  * [chubbyphp/chubbyphp-swoole-request-handler](https://github.com/chubbyphp/chubbyphp-swoole-request-handler) ⭐ 31 | 🐛 1 | 🌐 PHP | 📅 2026-07-20 - A request handler adapter for Swoole, using PSR-7, PSR-15 and PSR-17.
  * [fastd/http](https://github.com/fastdlabs/http) ⭐ 27 | 🐛 3 | 🌐 PHP | 📅 2026-08-08 - A PSR-7-compatible HTTP component, with built-in support for Swoole HTTP server. :globe\_with\_meridians:
  * [leocavalcante/request-callback](https://github.com/leocavalcante/request-callback) ⭐ 26 | 🐛 8 | 🌐 PHP | 📅 2022-11-08 - Swoole request callback for PSR compliant handlers. Compatible with PSR-7 and PSR-15.
  * [razonyang/psr7-swoole](https://github.com/razonyang/psr7-swoole) ⭐ 3 | 🐛 0 | 🌐 PHP | 📅 2022-09-24 - A PSR-7 helper for Swoole; a bridge between Swoole and PSR things, such as PSR-7 HTTP message, PSR-15 handlers and PSR-15 middlewares.

## Logging

* [upscale/swoole-newrelic](https://github.com/upscalesoftware/swoole-newrelic) ⭐ 16 | 🐛 1 | 🌐 PHP | 📅 2023-01-18 - New Relic APM and Browser monitoring of Swoole web-server.
* [hyperf/logger](https://github.com/hyperf/logger) ⭐ 4 | 🐛 0 | 🌐 PHP | 📅 2026-08-10 - The logging component of Hyperf. It's based on [Monolog](https://github.com/Seldaek/monolog) ⭐ 21,398 | 🐛 33 | 🌐 PHP | 📅 2026-08-01, with PSR-3 interface implemented.
* [mix/monolog](https://github.com/mix-php/monolog) ⭐ 1 | 🐛 0 | 🌐 PHP | 📅 2020-09-30 - A coroutine-friendly logging library. It's based on [Monolog](https://github.com/Seldaek/monolog) ⭐ 21,398 | 🐛 33 | 🌐 PHP | 📅 2026-08-01. :globe\_with\_meridians:
* [open-telemetry/context-swoole] - Async Swoole/OpenSwoole context implementation for OpenTelemetry PHP.

## Serverless

* [Swoole Runtime for AWS Lambda](https://github.com/leocavalcante/aws-lambda-swoole-runtime) ⭐ 41 | 🐛 0 | 🌐 PHP | 📅 2021-03-19 - λ Run PHP Coroutines & Fibers as-a-Service on the AWS Lambda.

## SOA governance

* [hyperf/tracer](https://github.com/hyperf/tracer) ⭐ 9 | 🐛 2 | 🌐 PHP | 📅 2026-08-10 - The distributed tracing component of Hyperf. The implementation is based on [OpenTracing](https://opentracing.io).
* [mix/tracing-zipkin](https://github.com/mix-php/tracing-zipkin) ⭐ 2 | 🐛 0 | 🌐 PHP | 📅 2020-09-30 - A tracing library based on [Zipkin](https://zipkin.io) and [OpenTracing](https://opentracing.io). :globe\_with\_meridians:

## Tasks and Queues

* [kcloze/swoole-jobs](https://github.com/kcloze/swoole-jobs) ⭐ 577 | 🐛 3 | 🌐 PHP | 📅 2022-11-30 - An efficient Swoole-based job queue system. :globe\_with\_meridians:
* [longlang/phpkafka](https://github.com/swoole/phpkafka) ⭐ 278 | 🐛 29 | 🌐 PHP | 📅 2024-02-21 - A coroutine-based [Kafka](https://kafka.apache.org) client.
* [Archer](https://github.com/swlib/archer) ⭐ 143 | 🐛 0 | 🌐 PHP | 📅 2020-07-17 - A Swoole-based task component, with different runtime modes supported: serial queue, concurrent queue, defer, timer, etc. :globe\_with\_meridians:
* [hyperf/amqp](https://github.com/hyperf/amqp) ⭐ 23 | 🐛 4 | 🌐 PHP | 📅 2026-06-07 - The AMQP client of Hyperf.
* [hyperf/async-queue](https://github.com/hyperf/async-queue) ⭐ 9 | 🐛 2 | 🌐 PHP | 📅 2026-07-26 - The Redis-based asynchronous queue component of Hyperf.
* [hyperf/task](https://github.com/hyperf/task) ⭐ 9 | 🐛 1 | 🌐 PHP | 📅 2026-06-07 - The task component of Hyperf, providing an easy way to add and dispatch tasks to task workers in Swoole.

## Testing

* [deminy/counit](https://github.com/deminy/counit) ⭐ 12 | 🐛 0 | 🌐 PHP | 📅 2026-07-28 - To run time/IO related unit tests (e.g., sleep function calls, database queries, API calls, etc) faster using Swoole.

## Third-party SDK

* [yansongda/pay](https://github.com/yansongda/pay) ⭐ 5,362 | 🐛 37 | 🌐 PHP | 📅 2026-08-14 - A payment SDK for Alipay and WeChat Pay, with components to integrate with [Hyperf](https://github.com/yansongda/hyperf-pay) ⭐ 91 | 🐛 2 | 🌐 PHP | 📅 2024-04-27, [Laravel](https://github.com/yansongda/laravel-pay) ⭐ 1,135 | 🐛 3 | 🌐 PHP | 📅 2026-03-19, and [Yii](https://github.com/guanguans/yii-pay) ⭐ 51 | 🐛 0 | 🌐 PHP | 📅 2026-05-02. :globe\_with\_meridians:
* [Yurunsoft/PaySDK](https://github.com/Yurunsoft/PaySDK) ⭐ 889 | 🐛 9 | 🌐 PHP | 📅 2026-07-19 - A coroutine-friendly payment SDK for Alipay and WeChat Pay. :globe\_with\_meridians:
* [Yurunsoft/YurunOAuthLogin](https://github.com/Yurunsoft/YurunOAuthLogin) ⭐ 434 | 🐛 2 | 🌐 PHP | 📅 2026-07-09 - An OAuth library that provides built-in support for QQ, WeChat, Weibo, Github, Gitee, etc. :globe\_with\_meridians:

## Web Applications

*Web-based applications and tools.*

* [HyperfAdmin](https://github.com/hyperf-admin/hyperf-admin) ⭐ 429 | 🐛 7 | 🌐 PHP | 📅 2023-04-18 - An administration panel built with Swoole, Hyperf, and Vue.js. :globe\_with\_meridians:
* [zhamao-framework](https://github.com/zhamao-robot/zhamao-framework) ⭐ 165 | 🐛 9 | 🌐 PHP | 📅 2026-08-12 - A chatbot system based on an award-winning project in China. :globe\_with\_meridians:
* [yurun-crawler](https://github.com/Yurunsoft/yurun-crawler) ⭐ 41 | 🐛 0 | 🌐 PHP | 📅 2020-11-04 - A framework to build high-performance, distributed web crawler. :globe\_with\_meridians:
* [wopits - A world of post-its](https://github.com/esaracco/wopits) ⚠️ Archived - An app for managing projects online using sticky notes to share and collaborate. It uses Swoole as a WebSocket & Task server.
* [MineAdmin] - An administration panel built with Swoole, Hyperf, and Vue 3. :globe\_with\_meridians:

## Miscellaneous

* [siteone-crawler](https://github.com/janreges/siteone-crawler) ⭐ 859 | 🐛 17 | 🌐 Rust | 📅 2026-06-29 - A fast Swoole-based cross-platform website crawler, cloner and analyzer for SEO, security, accessibility, and performance optimization - ideal for developers, DevOps and QA engineers. Supports Windows, macOS, and Linux. Also available as [desktop application](https://github.com/janreges/siteone-crawler-gui) ⭐ 248 | 🐛 17 | 🌐 Svelte | 📅 2025-06-09 based on Svelte + Electron.
* [hhxsv5/php-sse](https://github.com/hhxsv5/php-sse) ⭐ 457 | 🐛 7 | 🌐 PHP | 📅 2021-03-04 - A simple and efficient library implemented HTML5's server-sent events using PHP.
* [k8s/client](https://github.com/k8s-client/client) ⭐ 23 | 🐛 1 | 🌐 PHP | 📅 2023-01-28 - A Kubernetes API client for PHP.
* [crowdstar/exponential-backoff](https://github.com/Crowdstar/exponential-backoff) ⭐ 14 | 🐛 0 | 🌐 PHP | 📅 2026-04-19 - A library to prevent overloading an unavailable service by doubling the timeout each iteration. It works under both Swoole (in non-blocking mode) and PHP-FPM.
* [leocavalcante/swoole-mutex](https://github.com/leocavalcante/swoole-mutex) ⭐ 8 | 🐛 0 | 🌐 PHP | 📅 2020-04-11 - Mutual exclusion abstractions for PHP's Swoole concurrency run-time.
* [Shlink Event Dispatcher](https://github.com/shlinkio/shlink-event-dispatcher) ⭐ 4 | 🐛 0 | 🌐 PHP | 📅 2026-07-29 - Event dispatching using PSR-14, with async event listener that are executed in swoole task system.
* [mix/sync-invoke](https://github.com/mix-php/sync-invoke) ⭐ 3 | 🐛 0 | 🌐 PHP | 📅 2020-10-28 - A library to execute synchronous blocking code without blocking the running process in Swoole. :globe\_with\_meridians:
* Futures and Promises
  * [leocavalcante/swoole-futures](https://github.com/leocavalcante/swoole-futures) ⭐ 103 | 🐛 0 | 🌐 PHP | 📅 2020-04-08 - Futures + Async/Await for PHP's Swoole asynchronous run-time.
  * [Swoole Futures] - Partial implementation of Promise/A+ spec based on Swoole Coroutines.
* [Rubix ML] - A high-level machine learning and deep learning library for the PHP language.
* [xlswriter] - A coroutine-friendly PHP Extension to create and read XLSX files.

# Resources

## Swoole Books

*Fantastic Swoole-related books.*

* [Mastering Swoole PHP](https://www.amazon.com/Mastering-Swoole-PHP-performance-concurrent-ebook/dp/B0881B227S) - Build your high performance large scale concurrent system in a more flexible and efficient way than ever before with this first & only Swoole PHP book, with PHP 8 ready.
* [Swooleで学ぶPHP非同期処理　～並行処理／並列処理の基礎から実践的な開発手法まで一気にわかる](https://www.amazon.co.jp/-/en/%E3%82%81%E3%82%82%E3%82%8A%E3%83%BC/dp/429713358X) - Learning PHP asynchronous processing with Swoole: from the basics of parallel processing to practical development methods. The first Swoole book written in Japanese by [めもりー
  ](https://twitter.com/m3m0r7/) :globe\_with\_meridians:

## Swoole Videos

*Fantastic Swoole-related videos.*

* [CSP Programming in PHP](https://nomadphp.com/video/306/csp-programming-in-php) - An online talk presented by Demin on August 20, 2020. This talk gives an in depth explanation on the concurrency model used in Swoole. [Here](https://deminy.in/talks/csp.html) are the slides.
* [Building High-Performance Application Servers with Swoole](https://www.youtube.com/watch?v=fVdDB4mbGYQ) - A conference talk presented by Demin during PHPFest 2020. [Here](https://deminy.in/talks/phpfest2020.html) are the slides.
* [Build an All-In-One Application Server Using Swoole](https://www.youtube.com/watch?v=SJPZxvEYXxI\&t=1255s) - A conference talk presented by Demin during PHP Community Summit 2021. The talk starts at 20'55''. [Here](https://deminy.in/talks/pcs21.html) are the slides.

## Miscellaneous

* [deminy/swoole-by-examples](https://github.com/deminy/swoole-by-examples) ⭐ 214 | 🐛 0 | 🌐 PHP | 📅 2026-08-01 - Learn Swoole by examples.

[Consul]: https://en.wikipedia.org/wiki/Consul_\(software\)

[Elasticsearch]: https://www.elastic.co/elasticsearch

[friendsofhyperf/components]: https://github.com/friendsofhyperf/components

[MineAdmin]: https://github.com/mineadmin/MineAdmin

[open-telemetry/context-swoole]: https://github.com/opentelemetry-php/context-swoole

[Phluxor]: https://github.com/ytake/phluxor

[Rubix ML]: https://github.com/RubixML/ML

[Swoole Futures]: https://github.com/distantmagic/swoole-futures

[swoole-bundle/swoole-bundle]: https://github.com/symfony-swoole/swoole-bundle

[Utopia]: https://github.com/utopia-php/http

[xlswriter]: https://github.com/viest/php-ext-xlswriter

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-16._
