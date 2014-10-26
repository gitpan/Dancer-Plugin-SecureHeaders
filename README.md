# NAME

Dancer::Plugin::SecureHeaders - Automate HTTP Security headers.

# VERSION

Version 0.1.0

our $VERSION = '0.1.0';

# DESCRIPTION

Automatically add HTTP Security Headers to requests.

# SYNOPSIS

Provides sensible default HTTP Security headers. Allows setting the headers in the plugin configuration.

Will not override any headers set manually.

# SETTINGS

## Frame-Options

Sets the __X-Frame-Options__ header. Defaults to __"DENY"__.

## Content-Security-Policy

Sets the __X-Content-Security-Policy__ header. Defaults to __"default-src 'self'"__. 

Specification for this header is available at [https://dvcs.w3.org/hg/content-security-policy/raw-file/bcf1c45f312f/csp-unofficial-draft-20110303.html](https://dvcs.w3.org/hg/content-security-policy/raw-file/bcf1c45f312f/csp-unofficial-draft-20110303.html).

## IE-Settings

Determines whether to supplier IE-specific headers.

## IE-Content-Type-Options

Sets the __X-Content-Type-Options__ header for IE. Defaults to __"nosniff"__.

## IE-Download-Options

Sets the __X-Download-Options__ header for IE. Defaults to __'noopen'__.

## IE-XSS-Protection

Sets the __X-XSS-Protection__ header. Defaults to __"1; 'mode=block'"__.

# Example Settings (default)

# AUTHOR

Ewen, Colin, `<draecas at gmail.com>`

# BUGS

Please report any bugs or feature requests to `bug-dancer-plugin-secureheaders at rt.cpan.org`, or through
the web interface at [http://rt.cpan.org/NoAuth/ReportBug.html?Queue=Dancer-Plugin-SecureHeaders](http://rt.cpan.org/NoAuth/ReportBug.html?Queue=Dancer-Plugin-SecureHeaders).  I will be notified, and then you'll
automatically be notified of progress on your bug as I make changes.

# SUPPORT

You can find documentation for this module with the perldoc command.

    perldoc Dancer::Plugin::SecureHeaders

You can also look for information at:

- RT: CPAN's request tracker (report bugs here)

    [http://rt.cpan.org/NoAuth/Bugs.html?Dist=Dancer-Plugin-SecureHeaders](http://rt.cpan.org/NoAuth/Bugs.html?Dist=Dancer-Plugin-SecureHeaders)

- AnnoCPAN: Annotated CPAN documentation

    [http://annocpan.org/dist/Dancer-Plugin-SecureHeaders](http://annocpan.org/dist/Dancer-Plugin-SecureHeaders)

- CPAN Ratings

    [http://cpanratings.perl.org/d/Dancer-Plugin-SecureHeaders](http://cpanratings.perl.org/d/Dancer-Plugin-SecureHeaders)

- Search CPAN

    [http://search.cpan.org/dist/Dancer-Plugin-SecureHeaders/](http://search.cpan.org/dist/Dancer-Plugin-SecureHeaders/)

# ACKNOWLEDGEMENTS

# LICENSE AND COPYRIGHT

Copyright 2014 Ewen, Colin.

This program is free software; you can redistribute it and/or modify it
under the terms of the the Artistic License (2.0). You may obtain a
copy of the full license at:

[http://www.perlfoundation.org/artistic\_license\_2\_0](http://www.perlfoundation.org/artistic_license_2_0)

Any use, modification, and distribution of the Standard or Modified
Versions is governed by this Artistic License. By using, modifying or
distributing the Package, you accept this license. Do not use, modify,
or distribute the Package, if you do not accept this license.

If your Modified Version has been derived from a Modified Version made
by someone other than you, you are nevertheless required to ensure that
your Modified Version complies with the requirements of this license.

This license does not grant you the right to use any trademark, service
mark, tradename, or logo of the Copyright Holder.

This license includes the non-exclusive, worldwide, free-of-charge
patent license to make, have made, use, offer to sell, sell, import and
otherwise transfer the Package with respect to any patent claims
licensable by the Copyright Holder that are necessarily infringed by the
Package. If you institute patent litigation (including a cross-claim or
counterclaim) against any party alleging that the Package constitutes
direct or contributory patent infringement, then this Artistic License
to you shall terminate on the date that such litigation is filed.

Disclaimer of Warranty: THE PACKAGE IS PROVIDED BY THE COPYRIGHT HOLDER
AND CONTRIBUTORS "AS IS' AND WITHOUT ANY EXPRESS OR IMPLIED WARRANTIES.
THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
PURPOSE, OR NON-INFRINGEMENT ARE DISCLAIMED TO THE EXTENT PERMITTED BY
YOUR LOCAL LAW. UNLESS REQUIRED BY LAW, NO COPYRIGHT HOLDER OR
CONTRIBUTOR WILL BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, OR
CONSEQUENTIAL DAMAGES ARISING IN ANY WAY OUT OF THE USE OF THE PACKAGE,
EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
