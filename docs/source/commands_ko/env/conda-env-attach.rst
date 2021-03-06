
.. _env attach_ref:

conda env attach
=======================

.. raw:: html

   <PRE>
   <!-- Manpage converted by man2html 3.0.1 -->
   <B>CONDA(1)</B>                         User Commands                        <B>CONDA(1)</B>
   
   
   
   
   </PRE>
   <H2>NAME</H2><PRE>
          conda - conda env attach
   
   
   </PRE>
   <H2>DESCRIPTION</H2><PRE>
          usage: conda-env attach [-h] (<B>-n</B> NAME | <B>-r</B> REMOTE) [-p PATH] [--force]
   
          [--no-builds] [--json] [--debug] [--verbose]
                 notebook
   
          WARNING:  This  command  is  deprecated  in conda 4.4 and scheduled for
          removal in conda 4.5.
   
          Embeds information describing your conda environment into the  notebook
          metadata
   
   
   </PRE>
   <H2>OPTIONS</H2><PRE>
      <B>positional</B> <B>arguments:</B>
          notebook
                 notebook file
   
      <B>optional</B> <B>arguments:</B>
          <B>-h</B>, <B>--help</B>
                 Show this help message and exit.
   
          <B>-n</B> NAME, <B>--name</B> NAME
                 local environment definition
   
          <B>-r</B> REMOTE, <B>--remote</B> REMOTE
                 remote environment definition
   
          <B>-p</B> PATH, <B>--prefix</B> PATH
                 Full path to environment prefix
   
          <B>--force</B>
                 Replace existing environment definition
   
          <B>--no-builds</B>
                 Remove build specification from dependencies
   
          <B>--json</B> Report all output as json. Suitable for using conda programmati-
                 cally.
   
          <B>--debug</B>
                 Show debug output.
   
          <B>--verbose</B>, <B>-v</B>
                 Use once for info, twice for debug, three times for trace.
   
      <B>examples:</B>
                 conda env attach <B>-n</B> base  notebook.ipynb  conda  env  attach  <B>-r</B>
                 user/environment notebook.ipynb
   
   
   
   
   </PRE>
   <H2>Anaconda, Inc.                      3i 2018                           CONDA(1)</H2><PRE>
   </PRE>
