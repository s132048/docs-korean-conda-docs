
.. _env upload_ref:

conda env upload
=======================

.. raw:: html

   <PRE>
   <!-- Manpage converted by man2html 3.0.1 -->
   <B>CONDA(1)</B>                         User Commands                        <B>CONDA(1)</B>
   
   
   
   
   </PRE>
   <H2>NAME</H2><PRE>
          conda - conda env upload
   
   
   </PRE>
   <H2>DESCRIPTION</H2><PRE>
          usage:  conda-env  upload  [-h] [-n OLD_NAME] [-f FILE] [--summary SUM-
          MARY] [-q]
   
          [--json] [--debug] [--verbose]
                 [name]
   
          WARNING: This command is deprecated in  conda  4.4  and  scheduled  for
          removal in conda 4.5.
   
          Upload an environment to anaconda.org
   
   
   </PRE>
   <H2>OPTIONS</H2><PRE>
      <B>positional</B> <B>arguments:</B>
          name   environment definition
   
      <B>optional</B> <B>arguments:</B>
          <B>-h</B>, <B>--help</B>
                 Show this help message and exit.
   
          <B>-n</B> OLD_NAME, <B>--name</B> OLD_NAME
                 environment definition [Deprecated]
   
          <B>-f</B> FILE, <B>--file</B> FILE
                 environment definition file (default: environment.yml)
   
          <B>--summary</B> SUMMARY
                 Short summary of the environment
   
          <B>-q</B>, <B>--quiet</B>
   
          <B>--json</B> Report all output as json. Suitable for using conda programmati-
                 cally.
   
          <B>--debug</B>
                 Show debug output.
   
          <B>--verbose</B>, <B>-v</B>
                 Use once for info, twice for debug, three times for trace.
   
      <B>examples:</B>
                 conda env upload conda  env  upload  project  conda  env  upload
                 <B>--file=</B>/path/to/environment.yml       conda      env      upload
                 <B>--file=</B>/path/to/environment.yml project
   
   
   
   
   </PRE>
   <H2>Anaconda, Inc.                      3i 2018                           CONDA(1)</H2><PRE>
   </PRE>
