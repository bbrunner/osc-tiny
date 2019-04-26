Release Notes
=============

0.1.2
-----

* Added capability to add attributes

0.1.1
-----

* Added ``changereviewstate`` to list of allowed commands on
  :py:meth:`osctiny.bs_requests.Request.cmd`
* Added capability to add comments
* Added extension for build results
* Added :py:meth:`osctiny.packages.Package.checkout` to properly check-out an
  entire package
* Request parameters get encoded prior to submission to avoid decoding issues in
  the build service
* On initialization :py:class:`osctiny.Osc` accepts a ``cache`` keyword argument
  to save API responses in a cache dictionary. But requests with ``stream=True``
  are excluded from caching!