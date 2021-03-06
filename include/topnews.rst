.. class:: news

.. _erlport_mail_list:

`2015-01-02 </news/#erlport-mail-list>`_ New ErlPort mail list
  Thanks to `Duncan McGreggor <https://github.com/oubiwann>`_ the ErlPort mail
  list erlport@googlegroups.com (https://groups.google.com/d/forum/erlport) is
  now open for discussions!

.. class:: news

.. _erlport1.0.0alpha:

`2013-06-10 </news/#erlport1-0-0alpha>`_ Released ErlPort 1.0.0alpha
  After almost 2 years of development new `1.0.0alpha
  </downloads/#erlport-1-0-0alpha>`__ version of ErlPort library was released.

  New version of ErlPort helps develop applications which want to connect
  Erlang to `Python </docs/python.html>`__ or `Ruby </docs/ruby.html>`__ or
  want to use Erlang as a middleware for these two programming languages.

  Changes:

  - Redesigned as Erlang application
  - Added support for all recent `Python </docs/python.html>`_ versions
  - Added support for all recent `Ruby </docs/ruby.html>`_ versions
  - Added support for custom data types

  The following is an example ErlPort session for Python:

  .. sourcecode:: erl

    1> {ok, P} = python:start().
    {ok,<0.34.0>}
    2> python:call(P, sys, 'version.__str__', []).
    <<"2.7.3 (default, Aug  1 2012, 05:14:39) \n[GCC 4.6.3]">>
    3> python:call(P, operator, add, [2, 2]).
    4
    4> python:stop(P).
    ok

  Please check `Documentation </docs/>`__ page for more details about ErlPort
  and `Downloads </downloads/>`__ page for installation instructions and
  packages to download.

  .. class:: warning

  *WARNING: It's still an alpha version so expect bugs and backward
  incompatible changes in the future*
