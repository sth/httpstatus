# httpstatus

Shell scripts to check the HTTP status code for a URL

## Usage

`httpstatus` issues a HEAD request and returns the resulting status code
(the same status as your would get for a GET request):

    $ httpstatus 'https://tejp.de/'
	 200

`httpcheck` determines the status code and checks if it is an expected value.

    $ httpcheck 301 'http://tejp.de'

It exits with 0 if the status code was the expected value, otherwise it
shows an error message and exits with 1.
