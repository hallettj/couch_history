couch-history
==============

Utility to record your shell history in CouchDB. Based on [Shell Sink][] by
Josh Cronemeyer. This is alpha software and is under heavy development.

[Shell Sink]: http://shellsink.com/

To use install the script `_attachments/client/couch_history` somewhere in your
`$PATH` and include this line in your `.bashrc` configuration:

    export PROMPT_COMMAND="history | couch_history"

Make sure you have CouchDB running somewhere. By default couch_history stores
commands at http://localhost:5984/couch-history. To specify a different
location set an environment variable called `COUCH_HISTORY_URL`.


License
========

The MIT License

Copyright (c) 2009 Jesse Hallett <hallettj@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
