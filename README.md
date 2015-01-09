website
=======

Website for the course


# Deployment

In www/

	$ wintersmith build

	$ git add build

	$ git commit -m 'some update message'

	$ git push origin master

In project root

	$ git subtree push --prefix www/build origin gh-pages