## Sensu-Plugins-twilio

[![Build Status](https://travis-ci.org/sensu-plugins/sensu-plugins-twilio.svg?branch=master)](https://travis-ci.org/sensu-plugins/sensu-plugins-twilio)
[![Gem Version](https://badge.fury.io/rb/sensu-plugins-twilio.svg)](http://badge.fury.io/rb/sensu-plugins-twilio)
[![Code Climate](https://codeclimate.com/github/sensu-plugins/sensu-plugins-twilio/badges/gpa.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-twilio)
[![Test Coverage](https://codeclimate.com/github/sensu-plugins/sensu-plugins-twilio/badges/coverage.svg)](https://codeclimate.com/github/sensu-plugins/sensu-plugins-twilio)
[![Dependency Status](https://gemnasium.com/sensu-plugins/sensu-plugins-twilio.svg)](https://gemnasium.com/sensu-plugins/sensu-plugins-twilio)
[ ![Codeship Status for sensu-plugins/sensu-plugins-twilio](https://codeship.com/projects/879f33a0-dc04-0132-6ddb-025863fcc952/status?branch=master)](https://codeship.com/projects/79857)

## Functionality

## Files
 * bin/check-num-recordings.rb
 * bin/handler-twiliosms.rb

## Usage

```
{
  "twiliosms":{
    "token":"a9d8ag98daf98ga9fd8g",
    "number":"+111111111",
    "sid":"AC0ds98gd098gf09d8fg",
    "recipients":{
      "+11111111111": {
        "sensu_roles":[ "web-server" ], // subscribers
        "sensu_checks":[], // checks
        "sensu_level": 1 // 1 for warnging, 2 for critical alerts
      },
      "+11111222222": {
        "sensu_roles":[],
        "sensu_checks":[ "mysql-alive" ],
        "sensu_level": 2
      }
    }
  }
}
```
## Installation

[Installation and Setup](https://github.com/sensu-plugins/documentation/blob/master/user_docs/installation_instructions.md)

## Notes
