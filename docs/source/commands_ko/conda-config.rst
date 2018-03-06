
.. _config_ref:

conda config
=======================

.. raw:: html

   <PRE>
   <!-- Manpage converted by man2html 3.0.1 -->
   <B>CONDA(1)</B>                         User Commands                        <B>CONDA(1)</B>
   
   
   
   
   </PRE>
   <H2>NAME</H2><PRE>
          conda - conda config
   
   
   </PRE>
   <H2>DESCRIPTION</H2><PRE>
          usage: conda config [-h] [--json] [--debug] [--verbose]
   
          [--system | <B>--env</B> | <B>--file</B> FILE]
                 (<B>--show</B>  [SHOW  [SHOW  ...]]  |  <B>--show-sources</B>  |  <B>--validate</B> |
                 <B>--describe</B> [DESCRIBE [DESCRIBE ...]] | <B>--write-default</B>  |  <B>--get</B>
                 [KEY  [KEY  ...]]  |  <B>--append</B> KEY VALUE | <B>--prepend</B> KEY VALUE |
                 <B>--set</B> KEY VALUE |  <B>--remove</B>  KEY  VALUE  |  <B>--remove-key</B>  KEY  |
                 <B>--stdin</B>)
   
          Modify configuration values in .condarc.  This is modeled after the git
          config command.  Writes to the user .condarc file (<I>user</I> <I>.condarc</I>  <I>path</I>)
          by default.
   
   
   </PRE>
   <H2>OPTIONS</H2><PRE>
      <B>optional</B> <B>arguments:</B>
          <B>-h</B>, <B>--help</B>
                 Show this help message and exit.
   
          <B>--json</B> Report all output as json. Suitable for using conda programmati-
                 cally.
   
          <B>--debug</B>
                 Show debug output.
   
          <B>--verbose</B>, <B>-v</B>
                 Use once for info, twice for debug, three times for trace.
   
          <B>--system</B>
                 Write to the system .condarc file (root prefix/.condarc). Other-
                 wise writes to the user config file (<I>user</I> <I>.condarc</I> <I>path</I>).
   
          <B>--env</B>  Write  to the active conda environment .condarc file (&lt;no active
                 environment&gt;). If no environment is active, write  to  the  user
                 config file (<I>user</I> <I>.condarc</I> <I>path</I>).
   
          <B>--file</B> FILE
                 Write  to  the  given  file. Otherwise writes to the user config
                 file (<I>user</I> <I>.condarc</I> <I>path</I>) or the file path given  by  the  'CON-
                 DARC' environment variable, if it is set (default: <I>user</I> <I>.condarc</I>
                 <I>path</I>).
   
          <B>--show</B> [SHOW [SHOW ...]]
                 Display configuration values as calculated and compiled.  If  no
                 arguments  given, show information for all configuration values.
   
          <B>--show-sources</B>
                 Display all identified configuration sources.
   
          <B>--validate</B>
                 Validate all configuration sources.
   
          <B>--describe</B> [DESCRIBE [DESCRIBE ...]]
                 Describe given configuration parameters. If no arguments  given,
                 show information for all configuration parameters.
   
          <B>--write-default</B>
                 Write  the default configuration to a file. Equivalent to `conda
                 config <B>--describe</B> &gt; ~/.condarc`  when  no  <B>--env</B>,  <B>--system</B>,  or
                 <B>--file</B> flags are given.
   
          <B>--get</B> [KEY [KEY ...]]
                 Get a configuration value.
   
          <B>--append</B> KEY VALUE
                 Add one configuration value to the end of a list key.
   
          <B>--prepend</B> KEY VALUE, <B>--add</B> KEY VALUE
                 Add one configuration value to the beginning of a list key.
   
          <B>--set</B> KEY VALUE
                 Set a boolean or string key
   
          <B>--remove</B> KEY VALUE
                 Remove  a  configuration value from a list key. This removes all
                 instances of the value.
   
          <B>--remove-key</B> KEY
                 Remove a configuration key (and all its values).
   
          <B>--stdin</B>
                 Apply configuration  information  given  in  yaml  format  piped
                 through stdin.
   
                 See  `conda  config  <B>--describe</B>`  or  https://conda.io/docs/con-
                 fig.html for details on all the options that can go in .condarc.
   
                 Examples:
   
                 Display all configuration values as calculated and compiled:
   
                 conda config <B>--show</B>
   
                 Display all identified configuration sources:
   
                 conda config <B>--show-sources</B>
   
                 Describe all available configuration options:
   
                 conda config <B>--describe</B>
   
                 Add the conda-canary channel:
   
                 conda config <B>--add</B> channels conda-canary
   
                 Set the output verbosity to level 3 (highest):
   
                 conda config <B>--set</B> verbosity 3
   
                 Get the channels defined in the system .condarc:
   
                 conda config <B>--get</B> channels <B>--system</B>
   
                 Add the 'foo' Binstar channel:
   
                 conda config <B>--add</B> channels foo
   
                 Disable the 'show_channel_urls' option:
   
                 conda config <B>--set</B> show_channel_urls no
   
   
   
   
   </PRE>
   <H2>Anaconda, Inc.                      3i 2018                           CONDA(1)</H2><PRE>
   </PRE>
