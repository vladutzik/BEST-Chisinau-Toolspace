Instalation
===========
+ git clone this repository to your local directory
+ rename `specific.cfg.php_example` file to `specific.cfg.php` taking in account to change its variables (esspecialy for connection with DB)
+ install bestch_toolspace schema (provided in .sql file) to your local DB
+ go lo localhost/toolspace.best-chisinau.org/
+ try to log in with google account
+ activate your account from DB by changing in table users columns: role, approved, blocked

CHANGELOG
=========

2012
----

### August
* moved codebase to github

### July
* initial version ToolSpace , 2012-07-09


CONTRIBUTORS
============
* [bumbu](http://github.com/bumbu/)
* [Ananas](http://github.com/ana-balica)
* Buhito
* [Vlad Lednioff](https://github.com/unordinary)


TECHNICAL STUFF
===============
Status codes:
	200	OK
	400	Bad Request
	401	Unauthorized
	404	Not Found
	405	Method Not Allowed
	501	Not Implemented
	503	Service Unavailable

F3::HTTP_100;


TODO
====

Tasks list order:
 - file types
 - zipping big files
 - Add dragndrop zone into the thumbnails zone, upload files only there
 - Easier navigation from edit pages
 - Add versioning based on git pushes, and git tags
 	https://github.com/vitalets/bootstrap-editable/commit/217379b5838c5be659166bb50fc5e4776a7e1408
 	https://github.com/vitalets/bootstrap-editable/blob/master/bump-version
 - Teach somebody to upload files


== All pages ==
- Fullfill main page
- Files tracking
- Move all language variables into one place
- Make feedback form pretier (http://habrahabr.ru/post/148332/)

== Login page ==
- Enable back-up login
 - Send additional login information to newly accepted accounts

== After login page ==
- Show what is new in this version

== Edit page ==
 - If image has small width, then dissaprove button is at top
 - Dragndrop has strange behaviour
 - Move action buttons to bottom
 - Files relations
 - Users should be able to add/change title and tags and submit them for approval
 - Before adding new file. show in real time related/same files to prevent files duplications
 - Preview created thumbs
 - If too many tags, then they will not be visible

== Search page ==
 - If search is done by 2 or more tags, show in results files that have all tags, then all-1, then all-2...
 - Smart search (add search by author, date, and other details)
 == Details ==
  - Share link (to last version)
  - Report bad file/duplication/shit...
  - Asign different labels colors for different file types
  - Ability to download images in different sizes
  - Zooming for big pictures
  - Make modal box height adjustable to window height

== Accounts ==
 - add new user button

== Account edit ==
 - Stats, history, activity

== Architecture ==
 - Standartise reroutes (enchance menu module)
 - Clear temp directory (Keep uploaded files for no longer then X time)