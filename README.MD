# OAuth Web Print
Also refer to the following "[report](https://hackmd.io/EwFgxgZgHA7CBsBaAJgZnsRIKoIyIE4BWGZFAI2XnRpLCA==?view)".

## Prerequest
- python 2 or 3
- bower
- nodejs-legacy
- npm (for installing bower)
- python-dev, libcups2-dev (in debian-based system (other distros unknown); for installing pycups)

## Installation and Execution

Use Python 2,

```
$ virtualenv env
$ source env/bin/activate
$ pip install -r requirement.txt
$ bower install
```

Use Python 3,

```
$ python3 -m venv env
$ source env/bin/activate
$ pip install wheel
$ pip install -r requirement.txt
$ bower install
```

To launch the website,
```
$ python app.py
```

Init DB (Assume root user not password)
```
create database cnl;
use cnl;
CREATE TABLE `user` (
	`user_name` VarChar( 45 ) NULL,
	`user_fb_id` VarChar( 100 ) NOT NULL,
	PRIMARY KEY ( `user_fb_id` ) )
ENGINE = InnoDB;
```

## Copyright and License
Copyright 2017 CNL Group 7. Code released under MIT license.

Copyright 2015 Kaushik Raj. Code released under MIT license.

Copyright 2013-2015 Iron Summit Media Strategies, LLC. Code released under the [Apache 2.0](https://github.com/IronSummitMedia/startbootstrap-sb-admin-2/blob/gh-pages/LICENSE) license.
