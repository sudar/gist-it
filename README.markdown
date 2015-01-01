# gist-it

An AppEngine app to embed files from a github repository like a gist

http://github.com/robertkrimen/gist-it

### Try it

You can try it at [gist-it.sudarmuthu.com](http://gist-it.sudarmuthu.com)

### Usage

Launch a working example with:

	dev_appserver.py .

The gisting handler is located at ```app.py/dispatch_gist_it```

Associated the handler with a path is pretty easy, for example:

	wsgi_application = webapp.WSGIApplication( [
		( r'(.*)', dispatch_gist_it ),
	], debug=True )

### WordPress Plugin

There is also a [WordPress Plugin](http://sudarmuthu.com/wordpress/wp-github-gist), which allows you to embed gist and files from Github in your blog posts or pages.

### Testing

To run python unit2 tests:

	make test

To run perl tests (against a running server):

	make t

### Author

Robert Krimen (robertkrimen@gmail.com)

* http://github.com/robertkrimen
* http://search.cpan.org/~rokr/?R=D
