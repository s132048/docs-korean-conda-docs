
.. _search_ref:

conda search
=======================

.. raw:: html

   <PRE>
   <!-- Manpage converted by man2html 3.0.1 -->
   <B>CONDA(1)</B>                         User Commands                        <B>CONDA(1)</B>
   
   
   
   
   </PRE>
   <H2>NAME</H2><PRE>
          conda - conda search
   
   
   </PRE>
   <H2>DESCRIPTION</H2><PRE>
          usage: conda search [-h] [-n ENVIRONMENT | <B>-p</B> PATH] [-i] [-C]
   
          [--platform PLATFORM] [--reverse-dependency] [--offline]
                 [-c  CHANNEL]  [--override-channels]  [--json] [--debug] [--ver-
                 bose] [--use-local] [-k]
   
          Search for packages and display associated information.
   
                 The input is a MatchSpec, a query language for  conda  packages.
                 See examples below.
   
   
   </PRE>
   <H2>OPTIONS</H2><PRE>
      <B>optional</B> <B>arguments:</B>
          <B>-h</B>, <B>--help</B>
                 Show this help message and exit.
   
          <B>-n</B> ENVIRONMENT, <B>--name</B> ENVIRONMENT
                 Name of environment.
   
          <B>-p</B> PATH, <B>--prefix</B> PATH
                 Full path to environment prefix.
   
          <B>-i</B>, <B>--info</B>
                 Provide  detailed  information  about  each package.  Similar to
                 output of 'conda info package-name'.
   
          <B>-C</B>, <B>--use-index-cache</B>
                 Use cache of channel index files, even if it has expired.
   
          <B>--platform</B> PLATFORM
                 Search the given platform. Should be  formatted  like  'osx-64',
                 'linux-32',  'win-64',  and  so on. The default is to search the
                 current platform.
   
          <B>--reverse-dependency</B>
                 Perform a reverse dependency search. When using this  flag,  the
                 <B>--full-name</B> flag is recommended. Use 'conda info package' to see
                 the dependencies of a package.
   
          <B>--offline</B>
                 Offline mode, don't connect to the Internet.
   
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
   
          <B>--json</B> Report all output as json. Suitable for using conda programmati-
                 cally.
   
          <B>--debug</B>
                 Show debug output.
   
          <B>--verbose</B>, <B>-v</B>
                 Use once for info, twice for debug, three times for trace.
   
          <B>--use-local</B>
                 Use locally built packages.
   
          <B>-k</B>, <B>--insecure</B>
                 Allow conda to perform "insecure" SSL connections and transfers.
                 Equivalent to setting 'ssl_verify' to 'false'.
   
   
   </PRE>
   <H2>EXAMPLES</H2><PRE>
          Search for a specific package named 'scikit-learn':
   
                 conda search scikit-learn
   
          Search for packages containing 'scikit' in the package name:
   
                 conda search *scikit*
   
          Note  that your shell may expand '*' before handing the command over to
          conda.  Therefore it is sometimes necessary to  use  single  or  double
          quotes around the query.
   
                 conda search '*scikit' conda search "*scikit*"
   
          Search  for  packages  for  64-bit Linux (by default, packages for your
          current platform are shown):
   
                 conda search numpy[subdir=linux-64]
   
          Search for a specific version of a package:
   
                 conda search 'numpy&gt;=1.12'
   
          Search for a package on a specific channel
   
                 conda  search  conda-forge::numpy  conda   search   'numpy[chan-
                 nel=conda-forge, subdir=osx-64]'
   
   
   
   
   </PRE>
   <H2>Anaconda, Inc.                      3i 2018                           CONDA(1)</H2><PRE>
   </PRE>
