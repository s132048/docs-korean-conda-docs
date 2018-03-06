
.. _install_ref:

conda install
=======================

.. raw:: html

   <PRE>
   <!-- Manpage converted by man2html 3.0.1 -->
   <B>CONDA(1)</B>                         User Commands                        <B>CONDA(1)</B>
   
   
   
   
   </PRE>
   <H2>NAME</H2><PRE>
          conda - conda install
   
   
   </PRE>
   <H2>DESCRIPTION</H2><PRE>
          usage: conda install [-h] [--revision REVISION] [-y] [--dry-run] [-f]
   
          [--file FILE] [--no-deps] [--only-deps] [-m] [-C]
                 [--use-local]   [--offline]  [--no-pin]  [-c  CHANNEL]  [--over-
                 ride-channels] [-n ENVIRONMENT | <B>-p</B>  PATH]  [-q]  [--copy]  [-k]
                 [--update-dependencies]    [--no-update-dependencies]   [--chan-
                 nel-priority] [--no-channel-priority] [--clobber]  [--show-chan-
                 nel-urls]  [--no-show-channel-urls]  [--download-only]  [--json]
                 [--debug] [--verbose] [package_spec [package_spec ...]]
   
          Installs a list of packages into a specified conda environment.
   
                 This command accepts a  list  of  package  specifications  (e.g,
                 bitarray=0.8)  and  installs  a  set of packages consistent with
                 those specifications and compatible with the underlying environ-
                 ment.  If  full  compatibility  cannot  be  assured, an error is
                 reported and the environment is not changed.
   
                 Conda attempts to install the newest versions of  the  requested
                 packages.  To  accomplish this, it may update some packages that
                 are already installed, or install additional packages.  To  pre-
                 vent  existing  packages from updating, use the <B>--no-update-deps</B>
                 option. This may force conda to install older  versions  of  the
                 requested  packages,  and  it does not prevent additional depen-
                 dency packages from being installed.
   
                 If you wish to skip  dependency  checking  altogether,  use  the
                 '--force'  option. This may result in an environment with incom-
                 patible packages, so this option must be used  with  great  cau-
                 tion.
   
                 conda  can  also be called with a list of explicit conda package
                 filenames (e.g.  ./lxml-3.2.0-py27_0.tar.bz2).  Using  conda  in
                 this  mode  implies  the  <B>--force</B> option, and should likewise be
                 used with great caution. Explicit filenames and package specifi-
                 cations cannot be mixed in a single command.
   
   
   </PRE>
   <H2>OPTIONS</H2><PRE>
      <B>positional</B> <B>arguments:</B>
          package_spec
                 Packages to install or update in the conda environment.
   
      <B>optional</B> <B>arguments:</B>
          <B>-h</B>, <B>--help</B>
                 Show this help message and exit.
   
          <B>--revision</B> REVISION
                 Revert to the specified REVISION.
   
          <B>-y</B>, <B>--yes</B>
                 Do not ask for confirmation.
   
          <B>--dry-run</B>
                 Only display what would have been done.
   
          <B>-f</B>, <B>--force</B>
                 Force install (even when package already installed).
   
          <B>--file</B> FILE
                 Read  package versions from the given file. Repeated file speci-
                 fications can be passed (e.g. <B>--file</B>=<I>file1</I> <B>--file</B>=<I>file2</I>).
   
          <B>--no-deps</B>
                 Do not install, update, remove,  or  change  dependencies.  This
                 WILL  lead to broken environments and inconsistent behavior. Use
                 at your own risk.
   
          <B>--only-deps</B>
                 Only install dependencies.
   
          <B>-m</B>, <B>--mkdir</B>
                 Create the environment directory if necessary.
   
          <B>-C</B>, <B>--use-index-cache</B>
                 Use cache of channel index files, even if it has expired.
   
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
                 Name of environment.
   
          <B>-p</B> PATH, <B>--prefix</B> PATH
                 Full path to environment prefix.
   
          <B>-q</B>, <B>--quiet</B>
                 Do not display progress bar.
   
          <B>--copy</B> Install all packages using copies instead of hard- or soft-link-
                 ing.
   
          <B>-k</B>, <B>--insecure</B>
                 Allow conda to perform "insecure" SSL connections and transfers.
                 Equivalent to setting 'ssl_verify' to 'false'.
   
          <B>--update-dependencies</B>, <B>--update-deps</B>
                 Update  dependencies. Overrides the value given by `conda config
                 <B>--show</B> update_deps`.
   
          <B>--no-update-dependencies</B>, <B>--no-update-deps</B>
                 Don't update dependencies. Overrides the value given  by  `conda
                 config <B>--show</B> update_deps`.
   
          <B>--channel-priority</B>, <B>--channel-pri</B>, <B>--chan-pri</B>
                 Channel  priority  takes  precedence over package version. Over-
                 rides the value given by `conda config <B>--show</B> channel_priority`.
   
          <B>--no-channel-priority</B>, <B>--no-channel-pri</B>, <B>--no-chan-pri</B>
                 Package  version  takes  precedence over channel priority. Over-
                 rides the value given by `conda config <B>--show</B> channel_priority`.
   
          <B>--clobber</B>
                 Allow  clobbering of overlapping file paths within packages, and
                 suppress related warnings.
   
          <B>--show-channel-urls</B>
                 Show channel urls. Overrides the value given  by  `conda  config
                 <B>--show</B> show_channel_urls`.
   
          <B>--no-show-channel-urls</B>
                 Don't  show  channel  urls.  Overrides the value given by `conda
                 config <B>--show</B> show_channel_urls`.
   
          <B>--download-only</B>
                 Solve an environment and ensure package  caches  are  populated,
                 but  exit  prior to unlinking and linking packages into the pre-
                 fix.
   
          <B>--json</B> Report all output as json. Suitable for using conda programmati-
                 cally.
   
          <B>--debug</B>
                 Show debug output.
   
          <B>--verbose</B>, <B>-v</B>
                 Use once for info, twice for debug, three times for trace.
   
   
   </PRE>
   <H2>EXAMPLES</H2><PRE>
                 conda install -n myenv scipy
   
   
   
   
   </PRE>
   <H2>Anaconda, Inc.                      3i 2018                           CONDA(1)</H2><PRE>
   </PRE>
