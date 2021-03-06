
.. _update_ref:

conda update
=======================

.. raw:: html

   <PRE>
   <!-- Manpage converted by man2html 3.0.1 -->
   <B>CONDA(1)</B>                         User Commands                        <B>CONDA(1)</B>
   
   
   
   
   </PRE>
   <H2>NAME</H2><PRE>
          conda - conda update
   
   
   </PRE>
   <H2>DESCRIPTION</H2><PRE>
          usage:   conda   update   [-h]  [-y]  [--dry-run]  [-f]  [--file  FILE]
          [--no-deps] [-m]
   
          [--use-index-cache] [--use-local] [--offline] [--no-pin]
                 [-c CHANNEL] [--override-channels] [-n ENVIRONMENT  |  <B>-p</B>  PATH]
                 [-q]  [--copy] [--clobber] [-k] [--alt-hint] [--update-dependen-
                 cies]      [--no-update-dependencies]       [--channel-priority]
                 [--no-channel-priority]  [--show-channel-urls]  [--no-show-chan-
                 nel-urls] [--json] [--debug] [--verbose]  [--all]  [package_spec
                 [package_spec ...]]
   
          Updates conda packages to the latest compatible version.
   
          This  command  accepts  a list of package names and updates them to the
          latest versions that are compatible with  all  other  packages  in  the
          environment.
   
          Conda  attempts  to  install the newest versions of the requested pack-
          ages. To accomplish this, it may update some packages that are  already
          installed, or install additional packages. To prevent existing packages
          from updating, use the <B>--no-update-deps</B> option. This may force conda to
          install  older versions of the requested packages, and it does not pre-
          vent additional dependency packages from being installed.
   
          If you wish to skip dependency checking altogether, use  the  '--force'
          option.  This  may result in an environment with incompatible packages,
          so this option must be used with great caution.
   
   
   </PRE>
   <H2>OPTIONS</H2><PRE>
      <B>positional</B> <B>arguments:</B>
          package_spec
                 Packages to update in the conda environment.
   
      <B>optional</B> <B>arguments:</B>
          <B>-h</B>, <B>--help</B>
                 Show this help message and exit.
   
          <B>-y</B>, <B>--yes</B>
                 Do not ask for confirmation.
   
          <B>--dry-run</B>
                 Only display what would have been done.
   
          <B>-f</B>, <B>--force</B>
                 Force install (even when  package  already  installed),  implies
                 <B>--no-deps</B>.
   
          <B>--file</B> FILE
                 Read  package versions from the given file. Repeated file speci-
                 fications can be passed (e.g. <B>--file</B>=<I>file1</I> <B>--file</B>=<I>file2</I>).
   
          <B>--no-deps</B>
                 Do not install dependencies.
   
          <B>-m</B>, <B>--mkdir</B>
                 Create the environment directory if necessary.
   
          <B>--use-index-cache</B>
                 Use cache of channel index files.
   
          <B>--use-local</B>
                 Use locally built packages.
   
          <B>--offline</B>
                 Offline mode, don't connect to the Internet.
   
          <B>--no-pin</B>
                 Ignore pinned file.
   
          <B>-c</B> CHANNEL, <B>--channel</B> CHANNEL
                 Additional channel  to  search  for  packages.  These  are  URLs
                 searched  in  the  order  they  are given (including file:// for
                 local directories). Then, the defaults or channels from .condarc
                 are  searched (unless <B>--override-channels</B> is given). You can use
                 'defaults' to get the default packages for conda,  and  'system'
                 to  get  the  system  packages,  which  also takes .condarc into
                 account. You can also  use  any  name  and  the  .condarc  chan-
                 nel_alias  value will be prepended. The default channel_alias is
                 http://conda.anaconda.org/.
   
          <B>--override-channels</B>
                 Do not search default or .condarc channels. Requires  <B>--channel</B>.
   
          <B>-n</B> ENVIRONMENT, <B>--name</B> ENVIRONMENT
                 Name      of      environment      (in     root     prefix/envs:
                 /Users/joelkim/.conda/envs).
   
          <B>-p</B> PATH, <B>--prefix</B> PATH
                 Full  path   to   environment   prefix   (default:   <I>root</I>   <I>pre-</I>
                 <I>fix/envs/conda-docs</I>).
   
          <B>-q</B>, <B>--quiet</B>
                 Do not display progress bar.
   
          <B>--copy</B> Install all packages using copies instead of hard- or soft-link-
                 ing.
   
          <B>--clobber</B>
                 Allow clobbering of overlapping file paths within packages,  and
                 suppress related warnings.
   
          <B>-k</B>, <B>--insecure</B>
                 Allow  conda  to  perform  "insecure" SSL connections and trans-
                 fers.Equivalent to setting 'ssl_verify' to 'false'.
   
          <B>--alt-hint</B>
                 Use an alternate algorithm to generate an unsatisfiability hint.
   
          <B>--update-dependencies</B>, <B>--update-deps</B>
                 Update dependencies (default: True).
   
          <B>--no-update-dependencies</B>, <B>--no-update-deps</B>
                 Don't update dependencies (default: False).
   
          <B>--channel-priority</B>, <B>--channel-pri</B>, <B>--chan-pri</B>
                 Channel priority takes precedence over package version (default:
                 True). Note: This feature is in beta and may change in a  future
                 release.
   
          <B>--no-channel-priority</B>, <B>--no-channel-pri</B>, <B>--no-chan-pri</B>
                 Package version takes precedence over channel priority (default:
                 False). Note: This feature is in beta and may change in a future
                 release.
   
          <B>--show-channel-urls</B>
                 Show channel urls (default: None).
   
          <B>--no-show-channel-urls</B>
                 Don't show channel urls.
   
          <B>--json</B> Report all output as json. Suitable for using conda programmati-
                 cally.
   
          <B>--debug</B>
                 Show debug output.
   
          <B>--verbose</B>, <B>-v</B>
                 Use once for info, twice for debug, three times for trace.
   
          <B>--all</B>  Update all installed packages in the environment.
   
   
   </PRE>
   <H2>EXAMPLES</H2><PRE>
                 conda update -n myenv scipy
   
   
   
   
   </PRE>
   <H2>Anaconda, Inc.                      1i 2018                           CONDA(1)</H2><PRE>
   </PRE>
