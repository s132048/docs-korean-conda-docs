
.. _env export_ref:

conda env export
=======================

.. raw:: html

   <PRE>
   <!-- Manpage converted by man2html 3.0.1 -->
   <B>CONDA(1)</B>                         User Commands                        <B>CONDA(1)</B>
   
   
   
   
   </PRE>
   <H2>NAME</H2><PRE>
          conda - conda env export
   
   
   </PRE>
   <H2>DESCRIPTION</H2><PRE>
          usage: conda-env export [-h] [-c CHANNEL] [--override-channels]
   
          [-n ENVIRONMENT | <B>-p</B> PATH] [-f FILE] [--no-builds]
                 [--ignore-channels] [--json] [--debug] [--verbose]
   
          Export a given environment
   
   
   </PRE>
   <H2>OPTIONS</H2><PRE>
      <B>optional</B> <B>arguments:</B>
          <B>-h</B>, <B>--help</B>
                 Show this help message and exit.
   
          <B>-c</B> CHANNEL, <B>--channel</B> CHANNEL
                 Additional channel to include in the export
   
          <B>--override-channels</B>
                 Do not include .condarc channels
   
          <B>-n</B> ENVIRONMENT, <B>--name</B> ENVIRONMENT
                 Name of environment.
   
          <B>-p</B> PATH, <B>--prefix</B> PATH
                 Full path to environment prefix.
   
          <B>-f</B> FILE, <B>--file</B> FILE
   
          <B>--no-builds</B>
                 Remove build specification from dependencies
   
          <B>--ignore-channels</B>
                 Do not include channel names with package names.
   
          <B>--json</B> Report all output as json. Suitable for using conda programmati-
                 cally.
   
          <B>--debug</B>
                 Show debug output.
   
          <B>--verbose</B>, <B>-v</B>
                 Use once for info, twice for debug, three times for trace.
   
      <B>examples:</B>
                 conda env export conda env export <B>--file</B> SOME_FILE
   
   
   
   
   </PRE>
   <H2>Anaconda, Inc.                      3i 2018                           CONDA(1)</H2><PRE>
   </PRE>
