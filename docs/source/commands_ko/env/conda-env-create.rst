
.. _env create_ref:

conda env create
=======================

.. raw:: html

   <PRE>
   <!-- Manpage converted by man2html 3.0.1 -->
   <B>CONDA(1)</B>                         User Commands                        <B>CONDA(1)</B>
   
   
   
   
   </PRE>
   <H2>NAME</H2><PRE>
          conda - conda env create
   
   
   </PRE>
   <H2>DESCRIPTION</H2><PRE>
          usage: conda-env create [-h] [-f FILE] [-n ENVIRONMENT | <B>-p</B> PATH] [-q]
   
          [--force] [--json] [--debug] [--verbose]
                 [remote_definition]
   
          Create an environment based on an environment file
   
   
   </PRE>
   <H2>OPTIONS</H2><PRE>
      <B>positional</B> <B>arguments:</B>
          remote_definition
                 remote environment definition / IPython notebook
   
      <B>optional</B> <B>arguments:</B>
          <B>-h</B>, <B>--help</B>
                 Show this help message and exit.
   
          <B>-f</B> FILE, <B>--file</B> FILE
                 environment definition file (default: environment.yml)
   
          <B>-n</B> ENVIRONMENT, <B>--name</B> ENVIRONMENT
                 Name of environment.
   
          <B>-p</B> PATH, <B>--prefix</B> PATH
                 Full path to environment prefix.
   
          <B>-q</B>, <B>--quiet</B>
   
          <B>--force</B>
                 force  creation  of  environment (removing a previously existing
                 environment of the same name).
   
          <B>--json</B> Report all output as json. Suitable for using conda programmati-
                 cally.
   
          <B>--debug</B>
                 Show debug output.
   
          <B>--verbose</B>, <B>-v</B>
                 Use once for info, twice for debug, three times for trace.
   
      <B>examples:</B>
                 conda  env  create  conda  env  create  <B>-n</B> name conda env create
                 vader/deathstar  conda  env  create  <B>-f=</B>/path/to/environment.yml
                 conda env create <B>-f=</B>/path/to/requirements.txt <B>-n</B> deathstar conda
                 env  create  <B>-f=</B>/path/to/requirements.txt  <B>-p</B>   <I>/home/user/soft-</I>
                 <I>ware/deathstar</I>
   
   
   
   
   </PRE>
   <H2>Anaconda, Inc.                      3i 2018                           CONDA(1)</H2><PRE>
   </PRE>
