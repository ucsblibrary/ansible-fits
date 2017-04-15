ansible-fits
============

Install [FITS](https://projects.iq.harvard.edu/fits) on RHEL/CentOS

Variables
---------

- `download_dir` the directory FITS is initially downloaded to;
  defaults to `/tmp/fits-{{ fits_ver }}-build`.

- `fits_ver` the version of FITS to install; defaults to 0.8.4.

- `fits_256` the SHA-256 of the FITS zipball.

- `fits_url` the URL schema for downloading FITS; defaults to `http://projects.iq.harvard.edu/files/fits/files/fits-{{ fits_ver }}.zip`

Example Playbook
----------------

```yaml
- hosts: all
  roles:
    - role: ucsblibrary.fits
      become: yes
      fits_ver: 0.8.4
      fits_256: 6e623987385d596f80d4e4bbd0509107e8b550af52fa89c3aa99a37d14c4bf84
```

License
-------

This software is Copyright © 2017 The Regents of the University of
California. All Rights Reserved.

Permission to copy, modify, and distribute this software and its
documentation for educational, research and non-profit purposes,
without fee, and without a written agreement is hereby granted,
provided that the above copyright notice, this paragraph and the
following three paragraphs appear in all copies.

Permission to make commercial use of this software may be obtained by
contacting:

Technology Transfer Office
9500 Gilman Drive, Mail Code 0910
University of California
La Jolla, CA 92093-0910
(858) 534-5815
invent@ucsd.edu

This software program and documentation are copyrighted by The Regents
of the University of California. The software program and
documentation are supplied "as is", without any accompanying services
from The Regents. The Regents does not warrant that the operation of
the program will be uninterrupted or error-free. The end-user
understands that the program was developed for research purposes and
is advised not to rely exclusively on the program for any reason.

IN NO EVENT SHALL THE UNIVERSITY OF CALIFORNIA BE LIABLE TO ANY PARTY
FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES,
INCLUDING LOST PROFITS, ARISING OUT OF THE USE OF THIS SOFTWARE AND
ITS DOCUMENTATION, EVEN IF THE UNIVERSITY OF CALIFORNIA HAS BEEN
ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. THE UNIVERSITY OF
CALIFORNIA SPECIFICALLY DISCLAIMS ANY WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
A PARTICULAR PURPOSE.  THE SOFTWARE PROVIDED HEREUNDER IS ON AN "AS
IS" BASIS, AND THE UNIVERSITY OF CALIFORNIA HAS NO OBLIGATIONS TO
PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR MODIFICATIONS.
