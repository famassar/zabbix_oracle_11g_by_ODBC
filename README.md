# Oracle 11 Template for Zabbix 7

A Zabbix 7 template for monitoring Oracle 11 databases that are no longer supported by the official template, using the same macro layout as the built-in “Oracle by ODBC” template shipped with Zabbix. [web:1]

## Overview

This template provides monitoring for legacy Oracle Database 11 instances in Zabbix 7 by reusing the standard ODBC-based approach. [web:1]  
It targets environments where Oracle 11 is still in use but cannot rely on the official “Oracle by ODBC” template due to version support limitations. [web:1]

## Features

- Designed specifically for Oracle 11 databases monitored via ODBC. [web:1]  
- Follows the same macro naming conventions as the official “Oracle by ODBC” template. [web:1]  
- Provides an easy migration path from the official template for older Oracle instances. [web:1]

## Requirements

- Zabbix Server or Proxy version 7.x with ODBC support enabled. [web:1]  
- Working ODBC connectivity from the Zabbix host to the Oracle 11 database. [web:1]  
- A Zabbix host configured to use this template and the proper Oracle client/ODBC driver installed. [web:1]

## Macros

Configure the host-level macros exactly as in the built-in “Oracle by ODBC” template that ships with Zabbix. [web:1]  
Reuse the same connection, user, and password macros you already set for hosts that use the official template. [web:1]

## Installation

1. Import the template XML into Zabbix via **Configuration → Templates → Import**. [web:1]  
2. Attach the template to the host that represents your Oracle 11 database. [web:1]  
3. Set all required macros on the host following the values used for the “Oracle by ODBC” template. [web:1]

## Usage

After assigning the template and configuring the macros, Zabbix will begin collecting metrics from the Oracle 11 database via ODBC. [web:1]  
Use the standard Zabbix graphs, triggers, and latest data views to analyze database performance and availability. [web:1]
