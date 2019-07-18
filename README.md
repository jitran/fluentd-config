# FluentD Configuration

FluentD Version: 1.4.2+

This repository contains FluentD configuration examples for parsing docker and standard log files. It forwards logs to:
 * CloudWatch
 * S3
 * SumoLogic

It uses the forest plugin to dynamically generate config for the new input sources.

[conf.d](conf.d/) structure:
 * inputs are prefixed with **in-**
 * outputs are prefixed with **out-**
 * [conf.d/out.conf](conf.d/out.conf) defines the output sources

**Note: There are placeholder variables in the [conf.d](conf.d/) files that need to be updated.**

Plugins required:
* fluent-plugin-forest 0.3.3
* fluent-plugin-record-modifier 1.0.2
* fluent-plugin-cloudwatch-logs 0.7.1
* fluent-plugin-s3 1.1.2
* fluent-plugin-sumologic_output 1.0.2
