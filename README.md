# comment_system
A commenting system that accepts:
1. Name,
2. Email,
3. Comment and pulls in Gravatars.

Form submitting goes via Ajax and does basic client side validation.
Comments  append to the bottom of the comment thread.


//Create Database

CREATE TABLE IF NOT EXISTS `comments` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `name` varchar(40) NOT NULL,
  `email` varchar(60) NOT NULL,
  `comment` text NOT NULL,
  `id_post` int(11) NOT NULL,
  `date` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP,
  PRIMARY KEY (`id`)
