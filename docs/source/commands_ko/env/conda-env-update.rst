
.. _env update_ref:

conda env update
=======================

.. raw:: html

   <PRE>
   <!-- Manpage converted by man2html 3.0.1 -->
   <B>CONDA(1)</B>                         User Commands                        <B>CONDA(1)</B>
   
   
   
   
   </PRE>
   <H2>NAME</H2><PRE>
          conda - conda env update
   
   
   </PRE>
   <H2>DESCRIPTION</H2><PRE>
          usage:  conda-env  update  [-h]  [-n  ENVIRONMENT  | <B>-p</B> PATH] [-f FILE]
          [--prune]
   
          [-q] [--json] [--debug] [--verbose]
                 [remote_definition]
   
          Update the current environment based on environment file
   
   
   </PRE>
   <H2>OPTIONS</H2><PRE>
      <B>positional</B> <B>arguments:</B>
          remote_definition
                 remote environment definition / IPython notebook
   
      <B>optional</B> <B>arguments:</B>
          <B>-h</B>, <B>--help</B>
                 Show this help message and exit.
   
          <B>-n</B> ENVIRONMENT, <B>--name</B> ENVIRONMENT
                 Name of environment.
   
          <B>-p</B> PATH, <B>--prefix</B> PATH
                 Full path to environment prefix.
   
          <B>-f</B> FILE, <B>--file</B> FILE
                 environment definition (default: environment.yml)
   
          <B>--prune</B>
                 remove installed packages not defined in environment.yml
   
          <B>-q</B>, <B>--quiet</B>
   
          <B>--json</B> Report all output as json. Suitable for using conda programmati-
                 cally.
   
          <B>--debug</B>
                 Show debug output.
   
          <B>--verbose</B>, <B>-v</B>
                 Use once for info, twice for debug, three times for trace.
   
      <B>examples:</B>
                 conda  env  update  conda  env  update  <B>-n</B>=<I>foo</I>  conda env update
                 <B>-f=</B>/path/to/environment.yml   conda   env   update    <B>--name</B>=<I>foo</I>
                 <B>--file</B>=<I>environment</I>.yml conda env update vader/deathstar
   
   
   
   
   </PRE>
   <H2>Anaconda, Inc.                      3i 2018                           CONDA(1)</H2><PRE>
   </PRE>
