
# cljp-mysql

A ClojurePHP library for MySQL.

## Disclaimer

This does not work at the moment, and is just a tool to help with developing the
Clojure to PHP compiler (https://github.com/rodnaph/clj-php).

## Usage

```clojure
(ns example
  (:use cljp-mysql))

(def cnn (make-connection "localhost" "root" "" "my_db"))

(with-connection cnn
  (query " select * from table_name "))
```

