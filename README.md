# SWI-Prolog pack for processing MIME messages

This repository provides the pack `mime`,   which may be installed using
the following command on a  machine   where  the  required C development
tools are installed (e.g., Linux is fine):

    ?- pack_install(mime).

It provides `library(mime)`, based on the `maildrop` library.

## History

For a long time `library(mime)` was part  of the standard `clib` package
of SWI-Prolog. It was used for  decoding `multipart-mime` HTTP requests.
The library was a big overkill for this problem though. The current HTTP
framework provides a lightweight alternative. As   is,  we consider this
library  too  large,  having  too  many   dependencies  and  too  little
applications to justify it as a core component.


## License

The interface is licensed using the  BSD-2 license. The maildrop sources
have been made available to SWI-Prolog under the LGPL2 license.
