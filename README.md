# Video Chat Application

A full video chat widget that can be setup modified & changed to plug and play into your website or app.
The Video Component enables peer assisted networking using the Real Time Media Flow Protocol (RTMFP) within the Adobe Flash® Platform.

## Requirements

1. PHP
2. MYSQL
2. FLASH/FLEX EDITOR OF YOUR CHOUCE
3. WEB SERVER

## Installation

1. go to http://labs.adobe.com/technologies/cirrus/  and sign up for a developer key
2. Specify your developer key in DeveloperKey constant in VideoChatByEddyF.mxml
3. Specify the URL of your web service in WebServiceUrl constant in VideoChatByEddyF.mxml
4. Create the registration table 

CREATE TABLE IF NOT EXISTS `registrations` (
  `id` BIGINT(20) NOT NULL AUTO_INCREMENT,
  `appid` BIGINT(20) NOT NULL DEFAULT ’0′,
  `username` VARCHAR(60) NOT NULL DEFAULT ”,
  `identity` VARCHAR(120) NOT NULL DEFAULT ”,
  `updated` DATETIME NOT NULL DEFAULT ’0000-00-00 00:00:00′,
  PRIMARY KEY  (`id`),
  KEY `updated` (`updated`)
) ENGINE=MyISAM  DEFAULT CHARSET=latin1;

5. Run the application from two different browsers. 