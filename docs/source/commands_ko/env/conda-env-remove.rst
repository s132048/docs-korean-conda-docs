
.. _env remove_ref:

conda env remove
=======================

.. raw:: html

   <PRE>
   <!-- Manpage converted by man2html 3.0.1 -->
   <B>CONDA(1)</B>                         User Commands                        <B>CONDA(1)</B>
   
   
   
   
   </PRE>
   <H2>NAME</H2><PRE>
          conda - conda env remove
   
   
   </PRE>
   <H2>DESCRIPTION</H2><PRE>
          usage:  conda-env  remove  [-h]  [-n  ENVIRONMENT  |  <B>-p</B> PATH] [--json]
          [--debug]
   
                 [--verbose] [-q] [-y] [--dry-run]
   
          Remove an environmentRemoves a provided environment.  You must  deacti-
          vate the existing environment before you can remove it.
   
   
   </PRE>
   <H2>OPTIONS</H2><PRE>
      <B>optional</B> <B>arguments:</B>
          <B>-h</B>, <B>--help</B>
                 Show this help message and exit.
   
          <B>-n</B> ENVIRONMENT, <B>--name</B> ENVIRONMENT
                 Name of environment.
   
          <B>-p</B> PATH, <B>--prefix</B> PATH
                 Full path to environment prefix.
   
          <B>--json</B> Report all output as json. Suitable for using conda programmati-
                 cally.
   
          <B>--debug</B>
                 Show debug output.
   
          <B>--verbose</B>, <B>-v</B>
                 Use once for info, twice for debug, three times for trace.
   
          <B>-q</B>, <B>--quiet</B>
                 Do not display progress bar.
   
          <B>-y</B>, <B>--yes</B>
                 Do not ask for confirmation.
   
          <B>--dry-run</B>
                 Only display what would have been done.
   
   
   </PRE>
   <H2>EXAMPLES</H2><PRE>
                 conda env remove --name FOO conda env remove -n FOO
   
   
   
   
   </PRE>
   <H2>Anaconda, Inc.                      3i 2018                           CONDA(1)</H2><PRE>
   </PRE>
