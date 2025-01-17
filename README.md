/-------------
| fink HEAD
\-------------


/-------------
| fink 0.45.x
\-------------

0.45.6 "Fuhgeddaboudit" (2022-02-19)

        * Hot fix for #240. Don't break when Pre-Depends is empty.

0.45.5 "Fui" (2022-01-20)

        * Support for Pre-Depends.
        * Validator improvements.

0.45.4 "Fuji" (2021-11-03)

        * Support XQuartz 2.8+.

0.45.3 "No word" (2021-03-06)

        * Restore default path to /sw for 10.14 and earlier.
        * Populate INSTALLSITESCRIPT so Makemaker scripts work with perl5.28

0.45.2 "Fulminate" (2020-10-02)

        * Move default install path to /opt/sw
        * Support 10.15.6 (and .7)
        * Clean some regex code for newer perls
        * Support Xcode12

0.45.1 "Fumarole" (2020-03-28)
        * Fix finding cups headers on 10.14+
        * Support 10.15.2 - 10.15.4
        * Support user shells running zsh

0.45.0 "Funicular" (2019-08-05)
        * Support 10.14.5, 10.14.6, and 10.15
        * Fully support .app bundles on APFS systems
        * Caching cleanup
        * Support for latest versions of Xcode and clang

/-------------
| fink 0.44.x
\-------------

0.44.1 "Extreme Explosion" (2019-03-13)
        * Support 10.13.6
        * Bugfix: Update bzip2 source to Fink's SF.net repo.

0.44.0 "Dubious Debacle" (2019-01-13)
        * Support 10.14
        * Improve dpkg bootstrapping
        * Support for Java 10


/-------------
| fink 0.43.x
\-------------

0.43.1 "Political Balderdash" (2018-04-18)
        * Bugfix:  fink.info (and other base packages) can't use SHA256 because of upgrade
          deadlocks 
        * Support Darwin 17.5
        * Other fixes and enhancements (see the commits)

0.43.0 "Obvious Allegory" (2018-03-24)
        * selfupdate-git 
        * selfupdate-svn
        * --prefix flag
        * Support 10.13.1-4
        * Support Java 9.0.x
        * Support 2017 version of Java 1.6
        * Better checksum support
        * Other fixes and enhancements (see the commits)


/-------------
| fink 0.42.x
\-------------

0.42.0 "Hello Whitney" (2017-10-07)
        * Support 10.13.0
        * Retroactively add official support for 10.12.2-6
        * Support Java 9
        * Add %p/Library/Launch{Agents, Daemons} to legal directories
        * Other fixes and enhancements (see the commits)

/-------------
| fink 0.41.x
\-------------


0.41.1 "Jigsaw" (2017-11-13)
        * Support 10.12.1
        * Change system-xfree86* versioning to 3:<XQuartz version from receipt>-3, with 
          fallback to the current 2:7.2-2 if the receipt is missing.

0.41.0 "Backsaw" (2017-09-20)
        * Support 10.12 (Sierra)

/-------------
| fink 0.40.x
\-------------

Skipped.  The development branch for Sierra was prematurely tagged with a 0.40.99 git
version.

/-------------
| fink 0.39.x
\-------------

0.39.5 "Koloth" (2016-08-13)
        * Support 10.11.0-6
        * Bugfix in detecting variable marker ($) in RuntimeVars
        * Use otool-classic under Xcode 8 CL tools

0.39.4 "Morgan" (2016-07-29)
        * Support 10.11.0-5
        * Forbid the use of shell variables as RuntimeVars
        * Additional tweaks (see commits)

0.39.3 "Antilles" (2016-02-28)
        * Support 10.11.0-3
        * Output cleanup in various places (see commits)

0.39.2 "Sheridan" (2015-10-31)
        * Use system versions of tools (make, cp, chmod) in %{default_script}
        * Add Restrictive/GPL and related License forms for OpenSSL-linked packages.

0.39.1 "Pierce" (2015-10-03)
        * Properly support Apple's JavaForOSX2015-1
        * Bugfix: Downgrade errors during postinstall .deb migration to nonfatal warnings

0.39.0 "Pike" (2015-10-01)
        * Support OS 10.11
        * Switch 10.9, 10.10, and 10.11 to use the 10.9-libcxx tree.

/-------------
| fink 0.38.x
\-------------

0.38.8 "Canyonlands" (2015-10-01)
        * Last release to support 10.7 and 10.8.
        * Updated pkgconfig path handling.

0.38.7 "Bryce Canyon" (2015-08-15)
        * Support OS 10.10.4 and 10.10.5
        * Bugfix: Replace more version strings with version objects  so that 10.10+ do the 
          right thing under comparisons.
          * Avoids people seeing information about enabling the nonexistent unstable tree
                  on 10.7 and later.
          * Also prevent creation of %p/fink/dists/stable/crypto

0.38.6 "Black Canyon of the Gunnison" (2015-06-13)
        * Bugfix: Maximum Xcode version conditional for 10.9 was being applied
          to 10.(>=9) .
        * Bugfix: Fix Xcode.app version detection in Engine.pm not to warn when
          there is no installed Xcode.app .
        * Validation fix for empty Description field.
        * Bump max Mountain Lion kernel version to 12.6, even though that's still
          OS 10.8.5.

0.38.5 "Biscayne" (2015-05-13)
        * Support OS 10.10.3
        * Revert supporting /opt/X11 directly on 10.8+ to provide X11 virtuals. 
        * Remove cgi-pm from Provides.
        * Reduce flat-namespace linkage validation to give a warning rather 
          than a fatal error, since some packages require being built this way.
        * Fatal validation error for filename/install_name mismatch in Shlibs.
        * Validate package names in dependency lists.

0.38.4 "Big Bend" (2015-02-09)
        * Support OS 10.10.2
        * Issue warning if Xcode and Xcode CLI versions don't match.
        * Fail if 'dev-tools' virtual package disappears.
        * Support /opt/X11 directly on 10.8+. 
        * Improved --dotty-build output.
        * Other diagnostic improvements.

0.38.3 "Badlands" (2014-11-29)
        * Enable 10.10 bindist by default
        * Support OS 10.10.1
        * Make system-java* packages visible even if not installed.
        * Validator now allows for public libraries to use @rpath.
        * Bootstrap with perl-5.18.

0.38.2 "Arches" (2014-10-29)
        * dev-tools virtual package now requires /usr/include/
        * Validator check for flat-namespace linkage
        * Skip validation of virtual package .infos
        * Bugfix: 10.10 SDK option for 10.9/Xcode 6.1 now works
        * Bugfix: Use appropriate prefixes for Yosemite

0.38.1 "American Samoa" (2014-10-18)
        * Bugfix: restore Fink::CLI::prompt_selection to Engine.pm (removed accidentally
          in [9177185])
        * Add 10.10 SDK option for 10.9/Xcode 6.1.

0.38.0 "Acadia" (2014-10-18)
        * Support Yosemite (10.10)

/-------------
| fink 0.37.x
\-------------

0.37.1 "Alaska Assessor" (2014-09-20) 
        * Officially recognize OS 10.9.4.


0.37.0 "Alabama Antiquarian" (2014-06-03) 
        * First release not to support 10.6.
        * Officially recognize OS 10.9.3.
        * Install compiler wrappers in the .deb rather than autogenerating them.
        * Additional fixes and enhancements.

/-------------
| fink 0.36.x
\-------------

0.36.5 "Order today" (2014-06-03) 
        * Last release to support 10.6.
        * fix system-java detection for older Java versions.
        * Additional fixes and enhancements.

0.36.4.1 (2014-04-11)
        * Bugfix: change compiler wrapper test so that clang from Xcode 5.0 doesn't
          use -Wno-error=unused-command-line-argument-hard-error-in-future.

0.36.4 "Supplies are limited" (2014-04-06)
        * Activate official binary distributions. 
        * Official 10.9.2. support
        * Bootstrap on 10.6 defaults to 10.6/x86_64.
        * Tweak compiler wrappers to allow packages that pass flags that clang doesn't
          understand still to build with the Xcode 5.1 Command Line Tools.
          (-Wno-error=unused-command-line-argument-hard-error-in-future)
        * Bugfix: fix issue with bootstrapping with no Xcode.app installed.
        * Additional fixes  

0.36.3.1 (2013-12-30)
        * Bugfix: fix dpkg-lockwait and apt-get-lockwait on 10.6/i386
          by reverting the changes from dcf07ad27536cea139069ea3570a225bb91590b3
          only for that platform. 

0.36.3 "Order now, and we'll double the offer!" (2013-12-26)
        * Official 10.9.1 support.
        * Allow binary distributions to work for x86_64.
        * Other bugfixes and validator improvements.

0.36.1 "But wait, there's more!" (2013-11-17)
        * Bugfix: fix a perlmod build issue which crept in with 0.36.0.
        * Check for compatible CLI tools version in bootstrap.
        * Validator improvements.

0.36.0 "Watch this space" (2013-10-31)
        * Support OS 10.9.

/-------------
| fink 0.35.x
\-------------

0.35.2 "BYOB" (2013-09-26)
        * Bugfix: Fix bootstrap/build under 10.8/Xcode 5.
        * Support OS 10.8.5.
        * Bugfix: Fix 'fink dumpinfo' output for PatchFileN.
        * Validation::_min_fink_version() replaced by more generic
          Validation::_require_dep().

0.35.1 "BBQ" (2013-07-08)
        * Bugfix:  10.5-EOL was still visible.  Fix that.

0.35.0 "TLA" (2013-07-05)
        * First release to support only Snow Leopard (10.6) and later.
        * Support OS 10.8.4.
        * Add detection for Java-1.7.0.
        * Have fink display the help text if given an unknown verb.  This lets "fink help"
          and "fink --help" give the same output and reduces surprises. :-)
        * Prevent package builds/installs if there is no upgrade path between the prior
          Distribution and the current OS.
        * We appear to need the fixes from both 0.34.7 and 0.34.8 for hanging tar, so 
          we'll have both.
        * For MakeMaker builds:  Override the default "g(cc|++)2-4.2" compiler option 
          given by the system's Perl on 10.6 in favor of our "g(cc|++)" wrapper, since
          gcc-4.2 isn't present for clean Xcode 4.2 installs, and our wrapper is equivalent
          (and contains arch information) for Xcode 3.2.x.
        * Validation::_min_fink_version() API change to allow more generic dependencies.
          Example:  Depends: fink (>= 0.32) now automatically satisfies BuildDepends 
          fink (>= 0.32).  Similarly, Depends: automatically satisfies RuntimeDepends.

/-------------
| fink 0.34.x
\-------------

0.34.9 "recessed" (2013-07-05)
        * Last release to support Leopard (10.5.x).
        * Have fink display the help text if given an unknown verb.  This lets "fink help"
          and "fink --help" give the same output and reduces surprises. :-)
        * Prevent package builds/installs if there is no upgrade path between the prior
          Distribution and the current OS.
        * Validation::_min_fink_version() API change to allow more generic dependencies.
          Example:  Depends: fink (>= 0.32) now automatically satisfies BuildDepends 
          fink (>= 0.32).  Similarly, Depends: automatically satisfies RuntimeDepends.
=== in common with 0.35.0 ===
        * Support OS 10.8.4.
        * Add detection for Java-1.7.0.
        * We appear to need the fixes from both 0.34.7 and 0.34.8 for hanging tar, so 
          we'll have both.
        * For MakeMaker builds:  Override the default "g(cc|++)2-4.2" compiler option 
          given by the system's Perl on 10.6 in favor of our "g(cc|++)" wrapper, since
          gcc-4.2 isn't present for clean Xcode 4.2 installs, and our wrapper is equivalent
          (and contains arch information) for Xcode 3.2.x.

0.34.8 "duct tape" (2013-05-08)
        * More general fix to the hanging tar issue.  Thanks to Eric Gallager (cooljeanius)
          for suggesting and testing this option.  Thanks, also, to Murr.
        * Improved "fink list --dotty-build".
        * Suggest using "fink configure" when facing legacy fink.conf path issue.
        * clang and clang++ wrappers, mostly for 10.6/i386.
        * Other bugfixes.

0.34.7 "overhead track" (2013-03-29)
        * Bugfix: address issue where fink's tar hangs during unpack operations. Thanks to
          Peter Dyballa for the workaround.

0.34.6 "Hook and loop" (2013-03-16)
        * Support 10.8.3.
        * Clean up error reports from missing system commands.

0.34.5 "suction cup hook" (2013-01-28)
        * Fix clang virtual package detection against Xcode 4.6+.
        * Update 10.4/base and 10.7/base package description files to match latest versions
          in bootstrap.
        * Removed a number of spurious virtual perlmods.
        * Check for valid Buildpath and FetchAltDir during 'fink configure'.
        * Additional documentation.

0.34.4 "Ceiling Mount" (2012-09-25)
        * Support 10.8.2 and 10.7.5
        * Check permissions in working directories to make sure that fink-bld can
          operate.

0.34.3 "wall anchor" (2012-08-29)
        * Support 10.8.1.
        * Move Essential packages to gettext8.
        * Update 10.4/base and 10.7/base package description files to match latest versions
          in bootstrap.
        * Bugfixes
                * Fix .deb validator test for compiled perlmods.
                * Remove fontconfig2 and xft2 from x11 virtual package Provides,
                  since we're using Fink packages for those exclusively now.
                * Update fink.conf manpage to include Distribution: 10.8.

0.34.2 "magnetic" (2012-08-04)
        * Bugfixes
                * Fix test for unused UIDs/GIDs in Services.pm to allow checking
                  them separately.  This permits fink to restore the fink-bld user when
                  the Mountain Lion installer clobbers the user but not the group.
                * BuildAsNobody: false issues:
                  * Don't have fink-bld own directories in such cases.
                  * SplitOffs should inherit the same behavior as their parent.
                * Scrub a newline when finding the Developer directory via backticks
                  in AppBundles generation  (thanks to J. Steverud for the diagnosis).

0.34.1 "hanger" (2012-07-26)
        * Add a "pre-build-test.sh" script to check for system executables that fink
          needs.
          * Currently we test for presence and executability of /usr/bin/pod2man.
          * Modified the following to run pre-build-test.sh:
                  * fink.info.in -> fink-*.info
                  * inject.pl (replaces check from 0.34.0)
                  * bootstrap (replaces check from 0.34.0)
        * Bugfixes
                * Use the results of the 64-bit Intel check in bootstrap to determine
                  whether users are offered the option of a 64-bit install.
                * Remove virtual package for IPC::Run3 since no system Perl actually
                  provides it.
                * Restore ability to run SplitForks on app bundles when using Xcode 4.3 and later
                  by switching from hardcoded /Developer to a portable construct.
                * Fix parsing of indented TarFilesRename fields.
                * Fix order of entries in %p/var/lib/dpkg/info/<package>.md5sums .
        * Add this file to the files installed by fink.

0.34.0 "bracket" (2012-07-16)
        * Initial Mountain Lion support.
        * Refuse to bootstrap when /usr/bin/pod2man isn't executable.
        * Use only Apple- or Fink-provided helper applications, e.g. rsync
          rather than arbitrary, possibly broken, third-party ones.
        * The only downloader which is now provided by Apple is curl, so stop
          checking in /usr/bin for wget, aria2, ....

/-------------
| fink 0.33.x
\-------------

0.33.3 "Higgsino" (2012-07-05)
        * Bugfix: force fink to put temporary scripts in /tmp when building as
          fink-bld to avoid failures under "sudo -E -s" and "su -m". 
        * Generate the MD5sums of all of the files for a package.  These are available
          under %p/var/lib/dpkg/info/<package>.md5sums.
        * Suppress STDERR messages from xcodebuild for folks who insist on not
          having Xcode.app.
        * Have the Version for xcode (>=4.3.0) correspond to the entire version string
          from "pkgutil --pkg-info com.apple.pkg.DeveloperToolsCLI".
        * Bugfix: 0.33.3.1: fixes and performance improvements in the md5sum routine.
        * Bugfix: 0.33.3.2: more fixes for the md5sum generator

0.33.2 "sup squark" (2012-06-20)
        * Bugfix:
                * Use output from '/usr/libexec/java_home' to generate default 
                  JAVA_HOME for builds.
                * This works on 10.5-10.7, so it's probably going to change at some
                  point without warning. :-)
        * Better logic in checking for the expected gcc compilers.

0.33.1 "Wino" (2012-06-12)
        * Bug fixes:
                * Justin Hallett discovered that 'id' from coreutils-default and 
                  /usr/bin/id behave differently, which causes the fink-bld user
                  not to get set up properly.  Hardcoding /usr/bin/id solves this.
                * Fixed stray diagnostic message from system SDK detection (Thanks 
                  to Remko Scharoo for the report).

0.33.0 "selectron" (2012-06-11)
    * Recognize OS 10.7.4.
        * Make fink use --build-as-nobody by default.
                * move creation of fink-bld user, if not already present, into fink
                  rather than passwd(-fink-bld).
                * If not present, use 'fink configure' to set up the fink-bld user's
                  parameters, and it will be created on the next operation where a 
                  build could occur.
                * BuildAsNobody: false field for .info files where the package can't be 
                    built as nobody.
                * --no-build-as-nobody option for fink to override this default option 
                    and build as root.
        * %p/Library/Python is now a legal directory.
        * Modify the versioning of the "xcode" virtual package.
            * Version of the CLI Tools, if those are installed, for OS 10.7+.
            * Still the version of Xcode.app for Xcode 4.2.1-.
        * "xcode.app" virtual package indicates the presence of Xcode.app, and its 
          version is the version of the app for all Xcode versions.  
        * Diagnostic output modifications for packages that have UseMaxBuildJobs:
          false.

/-------------
| fink 0.32.x
\-------------

0.32.6 "unicycle" (2012-04-14)
        * Add validator support for 'BuildAsNobody: false' in preparation for
          making --build-as-nobody the default build method.

0.32.5 "spinning" (2012-04-07)
        * Supports bootstrap with only the Xcode Command Line Tools.
        * clang virtual package
        * llvm-gcc virtual package
        * Clean up gcc* virtual packages:
                * Get rid of compilers in the defaults list that aren't available
                  for any modern Xcode.
                * Use an OS version dependent list so that users can tell whether
                  they need to install a different Xcode or if the package is just
                  wrong. :-)
        * Bugfixes:
                  * Message concerning RuntimeDepends now mentions fink (>=0.32.0) 
                    rather than the less user-friendly (>=0.31.99.git).
                  * Have a default value if no system SDKs are found to avoid 
                    "unitialized value" errors.
                  * 0.32.5 -> 0.32.5.2: these updates didn't get applied.
                  * 0.32.5.2 -> 0.32.5.3:  10.7 needs gcc4.2, not gcc4.0.
                  * 0.32.5.3 -> 0.32.5.4:  Fix some regressions from master,
                    including bootstrap text.
                  * 0.32.5.5:  Fix bootstrap on PowerPC.

0.32.4 "pedicab" (2012-03-27)
        * Improved checksum validation.
        * Enhance Xcode 4.3 support via the use of syscalls rather than
          hardcoded paths.
                * Other locations for Xcode.app than just /Applications.
                * System SDK's now show up again.
        * Make list of potential system SDKs OS-version dependent rather than
          one list for everybody, to avoid user confusion if a package Bdeps
          on an SDK which is nonexistent for a given Xcode (immediate failure
          mention package unavailaibility versus more verbose message telling
          user to install that SDK from Xcode).  SDKs which can be installed
          will still give a message telling the user to install them from Xcode.

0.32.3 "velocipede" (2012-02-16)
        * Support Xcode 4.3

0.32.2 "ordinary" (2012-02-03)
        * Bugfix: flag to use pax as the unarchiver was not getting unset for
          the next SourceN.
        * Support OS 10.7.3.

0.32.1 "penny-farthing" (2012-01-26)
        * Bugfix: get_build_directory() needed to include tar.xz as an option or 
          packages with a simple Source: foo.tar.xz would fail.

0.32.0 "recumbent" (2012-01-25)
        * Added new "RuntimeDepends" field, any .info file that wants to use this
          feature must BuildDepend on fink (>= 0.32.0-1).
        * Improved package validator to reject .deb files including .hg / .git
          directories.
        * Improved package validator to detect some issues with percent expansions.
        * Cleaned up the code base, including removal of some dead code for old OS X
          version, and anything related to the AddShlibDeps .info field.
        * Updated fink and fink.conf man pages.
        * Disallow bootstrapping into /usr/local and any subdir of it.
        * Disallow bootstrapping on OS X 10.4 and older.
        * Removed the obsolete prebinding code (it was for OS X 10.4 and older).
        * Let 'tar' handle compressed tar files directly.  
        * xz archive support.
                * Includes validation check with 0.32 as minimum fink
                  version for .xz formatted archives.
                * Automatic unpacking source files in .tar.xz format.
                * Automatically install the xz package with no need to declare a 
                  BuildDepend when a SourceN is a .xz file.
        * Check Xcode version in bootstrap phase before actually creating a Fink tree.
        * Check for -I or -L pointing to the builddir or install dir in .pc files.
        * Diagnostic message improvements
                * Mention "passwd-fink-bld" instead of "passwd" when the fink-bld user
                  is absent, since there's no "passwd" on 10.7.
                * In error messages, suggest that users try rebuilds with MaxBuildJobs: 1
                  if that's set higher, and print MBJ in the system info.
                * Stress emailing only one Fink mailing list for bug reports.

/-------------
| fink 0.31.x (see https://github.com/fink/fink/tree/branch_0_31)
\-------------

0.31.6 "supine" (2012-01-03)
        * BugFixes: cvs proxy tunnel doesn't support 'user:password', so strip that
                                that from information passed via ProxyHTTP.
                                ext method doesn't support proxy tunneling.

0.31.5 "deceit" (2011-11-21)
        * BugFix: gcc-4.2 isn't available after clean installs of Xcode 4.2, so
          users weren't able to bootstrap on 10.6/Xcode 4.2.  Revert the compiler
          wrappers to point to gcc|g++ rather than (gcc|g++)-4.2.

0.31.4 "perfidy" (2011-10-28)
        * Synced base .info files against latest versions from dists.
        * Added support for Xcode 4.2 on Mac OS X 10.6.
        * Fixed bootstrap issue when GNU sed is in the PATH.
        * Updated mirror list.

0.31.3 "mendacity" (2011-10-12)
        * Added support for Mac OS X 10.7.2.
        * Added support for App Store version of Growl.app as well as legacy prefpane.

0.31.2 "perjury" (2011-09-26)
        * No longer enforce "BDep:fink>=0.24.12" for use of PatchFile (nothing older
          than that would be usable now anyway)
        * Building with the number of threads specified by MaxBuildJobs is now
          default (i.e. UseMaxBuildJobs: true is the default) unless 
          MaxBuildJobs: false is set.
        * InstallScript always disables UseMaxBuildJobs.

0.31.1 ""little white"" (2011-09-11)
        * Added support for Mac OS X 10.7.1.
        * Allow 32 bit systems to bootstrap on 10.6.
        * Simplified some code by taking advantage of the fact that the minimal
          supported OS version now is 10.5.
        * Bug fixes

0.31.0 "fib" (2011-07-20)
        * Added support for Mac OS X 10.7.
        * Dropped support for any Mac OS X version before 10.5. So 10.5, 10.6 and
          10.7 are the only supported OS X versions now.
        * Bug fixes

/-------------
| fink 0.30.x (see https://github.com/fink/fink/tree/branch_0_30)
\-------------

0.30.2 "Palin" (2011-07-11)
        * Last fink version for 10.4, and end of support for the OS.
        * Adds support for the 10.4-EOL subdirectory in dists.

0.30.1 "Hannity" (2011-06-28)

0.30.0 "Beck" (2011-04-30)

/-------------
| fink 0.29.x (see https://github.com/fink/fink/tree/branch_0_29)
\-------------

0.29.21 "Charter Oak" (2011-03-24)

0.29.20 "FirsTier" (2011-03-09)

0.29.19 "EarthStar" (2011-01-15)

0.29.18 "Darby" (2010-11-12)
        10.5/x86_64 only

0.29.17 "Tifton" (2010-11-11)

0.29.16 "K" (2010-11-09)

0.29.15 "Hillcrest" (2010-10-24)

0.29.14 "Bramble" (2010-10-19)

0.29.13 "Peninsula" (2010-07-01)

0.29.12 "TierOne" (2010-06-09)

0.29.11 "Greece and Portugal" (2010-06-02)

0.29.10 "Vantus" (2009-09-27)

0.29.9 "Dwelling House" (2009-08-28)

0.29.8 "Integrity" (2009-08-13)

0.29.7 "HBOS" (2009-06-10)

0.29.6 "New Frontier" (2009-05-20)

0.29.5 "Silverton" (2009-05-13)

0.29.4 (2009-05-12)
        again quickly replaced

0.29.3 (2009-05-12)
        quickly replaced

0.29.2 "IKB" (2009-04-14)

0.29.1 "Kaupthing" (2009-04-09)

0.29.0 "IndyMac" (2009-04-05)

/-------------
| fink 0.28.x (see https://github.com/fink/fink/tree/branch_0_28)
\-------------

New features:
        * Validate the shlibs field for consistency
        * Inclusion of .info file as a control file in the .deb
        * New selfupdate code to make future addition of methods easier
        * Automatic suggestion to run fink selfupdate if it hasn't been done in a while.
        * Remind user to selfupdate after enabling unstable
        * Display actual Distribution string in 'fink -V'
        * Use lftpget if available and appropriate
        * Private shared-library syntax in Shlibs

0.28.7 "Piltdown Man" (2009-02-19)

0.28.6 "The Philosopher's Stone" (2008-10-05)

0.28.5 "Spontaneous Generation" (2008-07-08)

0.28.4 "The Humors" (2008-06-29)

0.28.3 "Cold Fusion" (2008-06-20)

0.28.2 "N-ray" (2008-05-05)

0.28.1 "Phlogiston" (2008-03-11)

0.28.0 "Aether" (2008-01-20)

/-------------
| fink 0.27.x (see https://github.com/fink/fink/tree/branch_0_27)
\-------------

New features
        * fink --build-as-nobody tries to build as user fink-bld instead of nobody, which is reserved by the OS.
        * Timeouts for sluggish/stalled downloads.
        * Validator detects deficient checking of some script return codes in .info files.
        * New in 0.27.2, add conditionals support to Shlibs and ConfFiles field (requires using BuildDepends: fink (>= 0.27.2) or higher).

Bug fixes
        * Saner handling of virtual (Provides) packages directly from the fink command-line.
        * Better recovery when encountering an unprocessable .info file.
        * More reliable building perl-module packages (Type: perl passed -j1 in default InstallScript).
        * Improved detection of non-fink X11.
        * Safer management of communication between fink and apt-get.

0.27.16 "Defecaloesiophobia" (2008-07-08)

0.27.15 "Zemmiphobia" (2008-06-29)

0.27.14 "Liticaphobia" (2008-06-27)

0.27.13 "Triskaidekaphobia" (2008-06-22)

0.27.12 "Batrachophobia" (2008-06-20)

0.27.11 "Athazagoraphobia" (2008-02-17)

0.27.10 "Rhabdophobia" (2008-01-02)

0.27.9 "Paralipophobia" (2007-11-06)

0.27.8 "Ailurophobia" (2007-11-02)

0.27.7 "Potophobia" (2007-10-24)

0.27.6 "Hippopotomonstrosesquippedaliophobia" (2007-07-18)

0.27.5
        Never released to the public

0.27.4 "Kakorrhaphiophobia" (2007-07-10)

0.27.3 "Didaskaleinophobia" (2007-06-15)

0.27.2 "Blennophobia" (2007-06-10)

0.27.1 "Arachibutyrophobia" (2007-03-19)

0.27.0 "Gynophobia" (2007-03-17)

/-------------
| fink 0.26.x (see https://github.com/fink/fink/tree/branch_0_26)
\-------------

New features
        * Obsoletes support
        * Enable more than one Notify plugin at once
        * Type: -64bit, %lib, and %type_num[] (for building 64bit libs in parallel with 32bit libs)
        * new Distribution: field, which behaves like the Architecture: field
        * Change allowed filenames for .info file, to: invariant
          packagename, optionally followed by archname, optionally follwed by
          distribution, and finally optionally followed by either version or
          version-revision, each delimited by hyphens.
        * "fink configure" now allows to enable/disable the unstable tree
        * --dpkg-status and --all modes for fink cleanup
        * --tests mode to utilize InfoTest blocks
                * on Errors are fatal
                * warn Errors turn to warnings
        * --validate mode that causes packages to be validated
                * on Errors are fatal
                * warn Errors turn to warning
        * Info4 (added in 0.26.2)

0.26.4 "The Joy Luck Club" (2007-03-14)

0.26.3 "Divine Secrets of the Ya-Ya Sisterhood" (2007-03-08)

0.26.2 "Beaches" (2007-03-07)

0.26.1 "Thelma and Louise" (2007-01-22)

0.26.0 "Steel Magnolias" (2006-12-09)

/-------------
| fink 0.25.x (see https://github.com/fink/fink/tree/branch_0_25)
\-------------

New features
        * Incremental Indexing
        * SkipPrompts
                * Any more categories users would like?
        * Info3
                * Can indent nicely in .info files
                * No more support for RFC-822 multi-lines
                * Can put comments in pkglist fields
        * fast scanpackages with apt-ftparchive
        * auto-detection of country
        * Validator fixes:
                * detect InfoN property (should be wrapper)
        * New --trees option restricts fink to using .info files in the chosen tree(s).
        * new fink cleanup syntax
        * New --maintainer mode
        * New --log-output and --logfile flags to save transcripts of package building process
        * Integrated scanpackages, including ability to not index restrictive packages.
        * Support for running package test suites
        * reevaluate fink --tree=stable list
        * Validator:
                * Complain about > and < in dependency versioning (in .info).
                * dmacks: complete overhaul of .deb (val-unpack branch)
                * InfoN validator patch vasi fixed it the way he likes it
        * RangerRick: 'fink build foo-1.0-1' where a .deb exists in the bindist for foo-1.0-1 and UseBinaryDist is true should build locally, not fetch from the bindist.
        * Info3: allow comment lines in pkglist fields
        * "chown -h" functionality during --build-as-nobody (use Command:chowname_hr?)
        * dmacks: overhaul buildlocks to go away more automatically and have a cleaner cleanup
                * Automatically do cleanup when embarking on a package installation or removal
        * dmacks: buildlock destruction
                * Checking via lock_wait and PreRm
                * Removal on build failure via Fink::Finally
        * remove line-number in SysState error
        * BuildConflicts breakage
        * chown_hR is still leaving nobody-owned links.
        * progress bar during indexing ("." every 100 .info processed or
          every 10% of set of .info processed?) -- newbies to HEAD have
          complained index -f "has hung"...can take up to 5 minutes
        * alternate checksum algorithms

Bug fixes
        * Fink no longer gets confused by debs in a local apt repository
        * When asking to choose mirrors, fink orders choices alphabetically
          properly, and presents a reasonable set of mirrors when the user
          asks for all those on a continent.
        * BuildConflicts should actually work
        * many more we've forgotten all about...

0.25.3 "Reservoir Dogs" (2007-01-22)

0.25.2 "Things to Do in Denver When You're Dead" (2006-11-28)

0.25.1 "Road to Perdition" (2006-10-15)

0.25.0 "The Usual Suspects" (2006-09-17)

/-------------
| fink 0.24.x (see https://github.com/fink/fink/tree/branch_0_24)
\-------------

0.24.26 "Telescopium" (2006-08-12)

0.24.25 "Triangulum Australe" (2006-07-27)

0.24.24 "Norma [The Carpenter's Square]" (2006-07-20)

0.24.23 "Apus" (2006-07-03)

0.24.22 "Lupus" (2006-06-27)

0.24.21 "Boötes" (2006-06-23)

0.24.20 (2006-06-23)
        again quickly replaced

0.24.19 (2006-06-23)
        quickly replaced

0.24.18 "Circinus" (2006-06-12)

0.24.17 "Musca" (2006-05-31)

0.24.16 "Antlia" (2006-05-30)

0.24.15 "Hydra" (2006-03-27)

0.24.14 "Pyxis" (2006-03-21)

0.24.13
        Never released to the public

0.24.12 "Vulpecula" (2006-02-21)

0.24.11 "Lacerta" (2005-11-17)

0.24.10 "Cameloparadalis" (2005-08-25)

0.24.9 "Pavo" (2005-08-15)

0.24.8 "Coma Berenices" (2005-07-28)

0.24.7 "Carina" (2005-06-04)
        This release was made specifically for EOL'ing 10.2 support.

0.24.6 "Canes Venatici" (2005-05-11)

0.24.5 "Crux Austrialis" (2005-04-29)

0.24.4 "Ophiuchus" (2005-04-20)

0.24.3 "Cassiopeia" (2005-04-12)

0.24.2 "Draco" (2005-03-25)

0.24.1 "Ursa Major" (2005-02-28)

0.24.0 "Boilermaker" (2005-02-24)

/-------------
| fink 0.23.x (see https://github.com/fink/fink/tree/branch_0_23)
\-------------

/-------------
| fink 0.22.x (see https://github.com/fink/fink/tree/branch_0_22)
\-------------

/-------------
| fink 0.21.x (see https://github.com/fink/fink/tree/branch_0_21)
\-------------

/-------------
| fink 0.20.x (see https://github.com/fink/fink/tree/branch_0_20)
\-------------

/-------------
| fink 0.19.x (see https://github.com/fink/fink/tree/branch_0_19)
\-------------

/-------------
For a more comprehensive changelog of the latest experimental code, see:
        https://github.com/fink/fink/commits/

/-------------
| fink HEAD
\-------------


/-------------
| fink 0.45.x
\-------------

0.45.6 "Fuhgeddaboudit" (2022-02-19)

        * Hot fix for #240. Don't break when Pre-Depends is empty.

0.45.5 "Fui" (2022-01-20)

        * Support for Pre-Depends.
        * Validator improvements.

0.45.4 "Fuji" (2021-11-03)

        * Support XQuartz 2.8+.

0.45.3 "No word" (2021-03-06)

        * Restore default path to /sw for 10.14 and earlier.
        * Populate INSTALLSITESCRIPT so Makemaker scripts work with perl5.28

0.45.2 "Fulminate" (2020-10-02)

        * Move default install path to /opt/sw
        * Support 10.15.6 (and .7)
        * Clean some regex code for newer perls
        * Support Xcode12

0.45.1 "Fumarole" (2020-03-28)
        * Fix finding cups headers on 10.14+
        * Support 10.15.2 - 10.15.4
        * Support user shells running zsh

0.45.0 "Funicular" (2019-08-05)
        * Support 10.14.5, 10.14.6, and 10.15
        * Fully support .app bundles on APFS systems
        * Caching cleanup
        * Support for latest versions of Xcode and clang

/-------------
| fink 0.44.x
\-------------

0.44.1 "Extreme Explosion" (2019-03-13)
        * Support 10.13.6
        * Bugfix: Update bzip2 source to Fink's SF.net repo.

0.44.0 "Dubious Debacle" (2019-01-13)
        * Support 10.14
        * Improve dpkg bootstrapping
        * Support for Java 10


/-------------
| fink 0.43.x
\-------------

0.43.1 "Political Balderdash" (2018-04-18)
        * Bugfix:  fink.info (and other base packages) can't use SHA256 because of upgrade
          deadlocks 
        * Support Darwin 17.5
        * Other fixes and enhancements (see the commits)

0.43.0 "Obvious Allegory" (2018-03-24)
        * selfupdate-git 
        * selfupdate-svn
        * --prefix flag
        * Support 10.13.1-4
        * Support Java 9.0.x
        * Support 2017 version of Java 1.6
        * Better checksum support
        * Other fixes and enhancements (see the commits)


/-------------
| fink 0.42.x
\-------------

0.42.0 "Hello Whitney" (2017-10-07)
        * Support 10.13.0
        * Retroactively add official support for 10.12.2-6
        * Support Java 9
        * Add %p/Library/Launch{Agents, Daemons} to legal directories
        * Other fixes and enhancements (see the commits)

/-------------
| fink 0.41.x
\-------------


0.41.1 "Jigsaw" (2017-11-13)
        * Support 10.12.1
        * Change system-xfree86* versioning to 3:<XQuartz version from receipt>-3, with 
          fallback to the current 2:7.2-2 if the receipt is missing.

0.41.0 "Backsaw" (2017-09-20)
        * Support 10.12 (Sierra)

/-------------
| fink 0.40.x
\-------------

Skipped.  The development branch for Sierra was prematurely tagged with a 0.40.99 git
version.

/-------------
| fink 0.39.x
\-------------

0.39.5 "Koloth" (2016-08-13)
        * Support 10.11.0-6
        * Bugfix in detecting variable marker ($) in RuntimeVars
        * Use otool-classic under Xcode 8 CL tools

0.39.4 "Morgan" (2016-07-29)
        * Support 10.11.0-5
        * Forbid the use of shell variables as RuntimeVars
        * Additional tweaks (see commits)

0.39.3 "Antilles" (2016-02-28)
        * Support 10.11.0-3
        * Output cleanup in various places (see commits)

0.39.2 "Sheridan" (2015-10-31)
        * Use system versions of tools (make, cp, chmod) in %{default_script}
        * Add Restrictive/GPL and related License forms for OpenSSL-linked packages.

0.39.1 "Pierce" (2015-10-03)
        * Properly support Apple's JavaForOSX2015-1
        * Bugfix: Downgrade errors during postinstall .deb migration to nonfatal warnings

0.39.0 "Pike" (2015-10-01)
        * Support OS 10.11
        * Switch 10.9, 10.10, and 10.11 to use the 10.9-libcxx tree.

/-------------
| fink 0.38.x
\-------------

0.38.8 "Canyonlands" (2015-10-01)
        * Last release to support 10.7 and 10.8.
        * Updated pkgconfig path handling.

0.38.7 "Bryce Canyon" (2015-08-15)
        * Support OS 10.10.4 and 10.10.5
        * Bugfix: Replace more version strings with version objects  so that 10.10+ do the 
          right thing under comparisons.
          * Avoids people seeing information about enabling the nonexistent unstable tree
                  on 10.7 and later.
          * Also prevent creation of %p/fink/dists/stable/crypto

0.38.6 "Black Canyon of the Gunnison" (2015-06-13)
        * Bugfix: Maximum Xcode version conditional for 10.9 was being applied
          to 10.(>=9) .
        * Bugfix: Fix Xcode.app version detection in Engine.pm not to warn when
          there is no installed Xcode.app .
        * Validation fix for empty Description field.
        * Bump max Mountain Lion kernel version to 12.6, even though that's still
          OS 10.8.5.

0.38.5 "Biscayne" (2015-05-13)
        * Support OS 10.10.3
        * Revert supporting /opt/X11 directly on 10.8+ to provide X11 virtuals. 
        * Remove cgi-pm from Provides.
        * Reduce flat-namespace linkage validation to give a warning rather 
          than a fatal error, since some packages require being built this way.
        * Fatal validation error for filename/install_name mismatch in Shlibs.
        * Validate package names in dependency lists.

0.38.4 "Big Bend" (2015-02-09)
        * Support OS 10.10.2
        * Issue warning if Xcode and Xcode CLI versions don't match.
        * Fail if 'dev-tools' virtual package disappears.
        * Support /opt/X11 directly on 10.8+. 
        * Improved --dotty-build output.
        * Other diagnostic improvements.

0.38.3 "Badlands" (2014-11-29)
        * Enable 10.10 bindist by default
        * Support OS 10.10.1
        * Make system-java* packages visible even if not installed.
        * Validator now allows for public libraries to use @rpath.
        * Bootstrap with perl-5.18.

0.38.2 "Arches" (2014-10-29)
        * dev-tools virtual package now requires /usr/include/
        * Validator check for flat-namespace linkage
        * Skip validation of virtual package .infos
        * Bugfix: 10.10 SDK option for 10.9/Xcode 6.1 now works
        * Bugfix: Use appropriate prefixes for Yosemite

0.38.1 "American Samoa" (2014-10-18)
        * Bugfix: restore Fink::CLI::prompt_selection to Engine.pm (removed accidentally
          in [9177185])
        * Add 10.10 SDK option for 10.9/Xcode 6.1.

0.38.0 "Acadia" (2014-10-18)
        * Support Yosemite (10.10)

/-------------
| fink 0.37.x
\-------------

0.37.1 "Alaska Assessor" (2014-09-20) 
        * Officially recognize OS 10.9.4.


0.37.0 "Alabama Antiquarian" (2014-06-03) 
        * First release not to support 10.6.
        * Officially recognize OS 10.9.3.
        * Install compiler wrappers in the .deb rather than autogenerating them.
        * Additional fixes and enhancements.

/-------------
| fink 0.36.x
\-------------

0.36.5 "Order today" (2014-06-03) 
        * Last release to support 10.6.
        * fix system-java detection for older Java versions.
        * Additional fixes and enhancements.

0.36.4.1 (2014-04-11)
        * Bugfix: change compiler wrapper test so that clang from Xcode 5.0 doesn't
          use -Wno-error=unused-command-line-argument-hard-error-in-future.

0.36.4 "Supplies are limited" (2014-04-06)
        * Activate official binary distributions. 
        * Official 10.9.2. support
        * Bootstrap on 10.6 defaults to 10.6/x86_64.
        * Tweak compiler wrappers to allow packages that pass flags that clang doesn't
          understand still to build with the Xcode 5.1 Command Line Tools.
          (-Wno-error=unused-command-line-argument-hard-error-in-future)
        * Bugfix: fix issue with bootstrapping with no Xcode.app installed.
        * Additional fixes  

0.36.3.1 (2013-12-30)
        * Bugfix: fix dpkg-lockwait and apt-get-lockwait on 10.6/i386
          by reverting the changes from dcf07ad27536cea139069ea3570a225bb91590b3
          only for that platform. 

0.36.3 "Order now, and we'll double the offer!" (2013-12-26)
        * Official 10.9.1 support.
        * Allow binary distributions to work for x86_64.
        * Other bugfixes and validator improvements.

0.36.1 "But wait, there's more!" (2013-11-17)
        * Bugfix: fix a perlmod build issue which crept in with 0.36.0.
        * Check for compatible CLI tools version in bootstrap.
        * Validator improvements.

0.36.0 "Watch this space" (2013-10-31)
        * Support OS 10.9.

/-------------
| fink 0.35.x
\-------------

0.35.2 "BYOB" (2013-09-26)
        * Bugfix: Fix bootstrap/build under 10.8/Xcode 5.
        * Support OS 10.8.5.
        * Bugfix: Fix 'fink dumpinfo' output for PatchFileN.
        * Validation::_min_fink_version() replaced by more generic
          Validation::_require_dep().

0.35.1 "BBQ" (2013-07-08)
        * Bugfix:  10.5-EOL was still visible.  Fix that.

0.35.0 "TLA" (2013-07-05)
        * First release to support only Snow Leopard (10.6) and later.
        * Support OS 10.8.4.
        * Add detection for Java-1.7.0.
        * Have fink display the help text if given an unknown verb.  This lets "fink help"
          and "fink --help" give the same output and reduces surprises. :-)
        * Prevent package builds/installs if there is no upgrade path between the prior
          Distribution and the current OS.
        * We appear to need the fixes from both 0.34.7 and 0.34.8 for hanging tar, so 
          we'll have both.
        * For MakeMaker builds:  Override the default "g(cc|++)2-4.2" compiler option 
          given by the system's Perl on 10.6 in favor of our "g(cc|++)" wrapper, since
          gcc-4.2 isn't present for clean Xcode 4.2 installs, and our wrapper is equivalent
          (and contains arch information) for Xcode 3.2.x.
        * Validation::_min_fink_version() API change to allow more generic dependencies.
          Example:  Depends: fink (>= 0.32) now automatically satisfies BuildDepends 
          fink (>= 0.32).  Similarly, Depends: automatically satisfies RuntimeDepends.

/-------------
| fink 0.34.x
\-------------

0.34.9 "recessed" (2013-07-05)
        * Last release to support Leopard (10.5.x).
        * Have fink display the help text if given an unknown verb.  This lets "fink help"
          and "fink --help" give the same output and reduces surprises. :-)
        * Prevent package builds/installs if there is no upgrade path between the prior
          Distribution and the current OS.
        * Validation::_min_fink_version() API change to allow more generic dependencies.
          Example:  Depends: fink (>= 0.32) now automatically satisfies BuildDepends 
          fink (>= 0.32).  Similarly, Depends: automatically satisfies RuntimeDepends.
=== in common with 0.35.0 ===
        * Support OS 10.8.4.
        * Add detection for Java-1.7.0.
        * We appear to need the fixes from both 0.34.7 and 0.34.8 for hanging tar, so 
          we'll have both.
        * For MakeMaker builds:  Override the default "g(cc|++)2-4.2" compiler option 
          given by the system's Perl on 10.6 in favor of our "g(cc|++)" wrapper, since
          gcc-4.2 isn't present for clean Xcode 4.2 installs, and our wrapper is equivalent
          (and contains arch information) for Xcode 3.2.x.

0.34.8 "duct tape" (2013-05-08)
        * More general fix to the hanging tar issue.  Thanks to Eric Gallager (cooljeanius)
          for suggesting and testing this option.  Thanks, also, to Murr.
        * Improved "fink list --dotty-build".
        * Suggest using "fink configure" when facing legacy fink.conf path issue.
        * clang and clang++ wrappers, mostly for 10.6/i386.
        * Other bugfixes.

0.34.7 "overhead track" (2013-03-29)
        * Bugfix: address issue where fink's tar hangs during unpack operations. Thanks to
          Peter Dyballa for the workaround.

0.34.6 "Hook and loop" (2013-03-16)
        * Support 10.8.3.
        * Clean up error reports from missing system commands.

0.34.5 "suction cup hook" (2013-01-28)
        * Fix clang virtual package detection against Xcode 4.6+.
        * Update 10.4/base and 10.7/base package description files to match latest versions
          in bootstrap.
        * Removed a number of spurious virtual perlmods.
        * Check for valid Buildpath and FetchAltDir during 'fink configure'.
        * Additional documentation.

0.34.4 "Ceiling Mount" (2012-09-25)
        * Support 10.8.2 and 10.7.5
        * Check permissions in working directories to make sure that fink-bld can
          operate.

0.34.3 "wall anchor" (2012-08-29)
        * Support 10.8.1.
        * Move Essential packages to gettext8.
        * Update 10.4/base and 10.7/base package description files to match latest versions
          in bootstrap.
        * Bugfixes
                * Fix .deb validator test for compiled perlmods.
                * Remove fontconfig2 and xft2 from x11 virtual package Provides,
                  since we're using Fink packages for those exclusively now.
                * Update fink.conf manpage to include Distribution: 10.8.

0.34.2 "magnetic" (2012-08-04)
        * Bugfixes
                * Fix test for unused UIDs/GIDs in Services.pm to allow checking
                  them separately.  This permits fink to restore the fink-bld user when
                  the Mountain Lion installer clobbers the user but not the group.
                * BuildAsNobody: false issues:
                  * Don't have fink-bld own directories in such cases.
                  * SplitOffs should inherit the same behavior as their parent.
                * Scrub a newline when finding the Developer directory via backticks
                  in AppBundles generation  (thanks to J. Steverud for the diagnosis).

0.34.1 "hanger" (2012-07-26)
        * Add a "pre-build-test.sh" script to check for system executables that fink
          needs.
          * Currently we test for presence and executability of /usr/bin/pod2man.
          * Modified the following to run pre-build-test.sh:
                  * fink.info.in -> fink-*.info
                  * inject.pl (replaces check from 0.34.0)
                  * bootstrap (replaces check from 0.34.0)
        * Bugfixes
                * Use the results of the 64-bit Intel check in bootstrap to determine
                  whether users are offered the option of a 64-bit install.
                * Remove virtual package for IPC::Run3 since no system Perl actually
                  provides it.
                * Restore ability to run SplitForks on app bundles when using Xcode 4.3 and later
                  by switching from hardcoded /Developer to a portable construct.
                * Fix parsing of indented TarFilesRename fields.
                * Fix order of entries in %p/var/lib/dpkg/info/<package>.md5sums .
        * Add this file to the files installed by fink.

0.34.0 "bracket" (2012-07-16)
        * Initial Mountain Lion support.
        * Refuse to bootstrap when /usr/bin/pod2man isn't executable.
        * Use only Apple- or Fink-provided helper applications, e.g. rsync
          rather than arbitrary, possibly broken, third-party ones.
        * The only downloader which is now provided by Apple is curl, so stop
          checking in /usr/bin for wget, aria2, ....

/-------------
| fink 0.33.x
\-------------

0.33.3 "Higgsino" (2012-07-05)
        * Bugfix: force fink to put temporary scripts in /tmp when building as
          fink-bld to avoid failures under "sudo -E -s" and "su -m". 
        * Generate the MD5sums of all of the files for a package.  These are available
          under %p/var/lib/dpkg/info/<package>.md5sums.
        * Suppress STDERR messages from xcodebuild for folks who insist on not
          having Xcode.app.
        * Have the Version for xcode (>=4.3.0) correspond to the entire version string
          from "pkgutil --pkg-info com.apple.pkg.DeveloperToolsCLI".
        * Bugfix: 0.33.3.1: fixes and performance improvements in the md5sum routine.
        * Bugfix: 0.33.3.2: more fixes for the md5sum generator

0.33.2 "sup squark" (2012-06-20)
        * Bugfix:
                * Use output from '/usr/libexec/java_home' to generate default 
                  JAVA_HOME for builds.
                * This works on 10.5-10.7, so it's probably going to change at some
                  point without warning. :-)
        * Better logic in checking for the expected gcc compilers.

0.33.1 "Wino" (2012-06-12)
        * Bug fixes:
                * Justin Hallett discovered that 'id' from coreutils-default and 
                  /usr/bin/id behave differently, which causes the fink-bld user
                  not to get set up properly.  Hardcoding /usr/bin/id solves this.
                * Fixed stray diagnostic message from system SDK detection (Thanks 
                  to Remko Scharoo for the report).

0.33.0 "selectron" (2012-06-11)
    * Recognize OS 10.7.4.
        * Make fink use --build-as-nobody by default.
                * move creation of fink-bld user, if not already present, into fink
                  rather than passwd(-fink-bld).
                * If not present, use 'fink configure' to set up the fink-bld user's
                  parameters, and it will be created on the next operation where a 
                  build could occur.
                * BuildAsNobody: false field for .info files where the package can't be 
                    built as nobody.
                * --no-build-as-nobody option for fink to override this default option 
                    and build as root.
        * %p/Library/Python is now a legal directory.
        * Modify the versioning of the "xcode" virtual package.
            * Version of the CLI Tools, if those are installed, for OS 10.7+.
            * Still the version of Xcode.app for Xcode 4.2.1-.
        * "xcode.app" virtual package indicates the presence of Xcode.app, and its 
          version is the version of the app for all Xcode versions.  
        * Diagnostic output modifications for packages that have UseMaxBuildJobs:
          false.

/-------------
| fink 0.32.x
\-------------

0.32.6 "unicycle" (2012-04-14)
        * Add validator support for 'BuildAsNobody: false' in preparation for
          making --build-as-nobody the default build method.

0.32.5 "spinning" (2012-04-07)
        * Supports bootstrap with only the Xcode Command Line Tools.
        * clang virtual package
        * llvm-gcc virtual package
        * Clean up gcc* virtual packages:
                * Get rid of compilers in the defaults list that aren't available
                  for any modern Xcode.
                * Use an OS version dependent list so that users can tell whether
                  they need to install a different Xcode or if the package is just
                  wrong. :-)
        * Bugfixes:
                  * Message concerning RuntimeDepends now mentions fink (>=0.32.0) 
                    rather than the less user-friendly (>=0.31.99.git).
                  * Have a default value if no system SDKs are found to avoid 
                    "unitialized value" errors.
                  * 0.32.5 -> 0.32.5.2: these updates didn't get applied.
                  * 0.32.5.2 -> 0.32.5.3:  10.7 needs gcc4.2, not gcc4.0.
                  * 0.32.5.3 -> 0.32.5.4:  Fix some regressions from master,
                    including bootstrap text.
                  * 0.32.5.5:  Fix bootstrap on PowerPC.

0.32.4 "pedicab" (2012-03-27)
        * Improved checksum validation.
        * Enhance Xcode 4.3 support via the use of syscalls rather than
          hardcoded paths.
                * Other locations for Xcode.app than just /Applications.
                * System SDK's now show up again.
        * Make list of potential system SDKs OS-version dependent rather than
          one list for everybody, to avoid user confusion if a package Bdeps
          on an SDK which is nonexistent for a given Xcode (immediate failure
          mention package unavailaibility versus more verbose message telling
          user to install that SDK from Xcode).  SDKs which can be installed
          will still give a message telling the user to install them from Xcode.

0.32.3 "velocipede" (2012-02-16)
        * Support Xcode 4.3

0.32.2 "ordinary" (2012-02-03)
        * Bugfix: flag to use pax as the unarchiver was not getting unset for
          the next SourceN.
        * Support OS 10.7.3.

0.32.1 "penny-farthing" (2012-01-26)
        * Bugfix: get_build_directory() needed to include tar.xz as an option or 
          packages with a simple Source: foo.tar.xz would fail.

0.32.0 "recumbent" (2012-01-25)
        * Added new "RuntimeDepends" field, any .info file that wants to use this
          feature must BuildDepend on fink (>= 0.32.0-1).
        * Improved package validator to reject .deb files including .hg / .git
          directories.
        * Improved package validator to detect some issues with percent expansions.
        * Cleaned up the code base, including removal of some dead code for old OS X
          version, and anything related to the AddShlibDeps .info field.
        * Updated fink and fink.conf man pages.
        * Disallow bootstrapping into /usr/local and any subdir of it.
        * Disallow bootstrapping on OS X 10.4 and older.
        * Removed the obsolete prebinding code (it was for OS X 10.4 and older).
        * Let 'tar' handle compressed tar files directly.  
        * xz archive support.
                * Includes validation check with 0.32 as minimum fink
                  version for .xz formatted archives.
                * Automatic unpacking source files in .tar.xz format.
                * Automatically install the xz package with no need to declare a 
                  BuildDepend when a SourceN is a .xz file.
        * Check Xcode version in bootstrap phase before actually creating a Fink tree.
        * Check for -I or -L pointing to the builddir or install dir in .pc files.
        * Diagnostic message improvements
                * Mention "passwd-fink-bld" instead of "passwd" when the fink-bld user
                  is absent, since there's no "passwd" on 10.7.
                * In error messages, suggest that users try rebuilds with MaxBuildJobs: 1
                  if that's set higher, and print MBJ in the system info.
                * Stress emailing only one Fink mailing list for bug reports.

/-------------
| fink 0.31.x (see https://github.com/fink/fink/tree/branch_0_31)
\-------------

0.31.6 "supine" (2012-01-03)
        * BugFixes: cvs proxy tunnel doesn't support 'user:password', so strip that
                                that from information passed via ProxyHTTP.
                                ext method doesn't support proxy tunneling.

0.31.5 "deceit" (2011-11-21)
        * BugFix: gcc-4.2 isn't available after clean installs of Xcode 4.2, so
          users weren't able to bootstrap on 10.6/Xcode 4.2.  Revert the compiler
          wrappers to point to gcc|g++ rather than (gcc|g++)-4.2.

0.31.4 "perfidy" (2011-10-28)
        * Synced base .info files against latest versions from dists.
        * Added support for Xcode 4.2 on Mac OS X 10.6.
        * Fixed bootstrap issue when GNU sed is in the PATH.
        * Updated mirror list.

0.31.3 "mendacity" (2011-10-12)
        * Added support for Mac OS X 10.7.2.
        * Added support for App Store version of Growl.app as well as legacy prefpane.

0.31.2 "perjury" (2011-09-26)
        * No longer enforce "BDep:fink>=0.24.12" for use of PatchFile (nothing older
          than that would be usable now anyway)
        * Building with the number of threads specified by MaxBuildJobs is now
          default (i.e. UseMaxBuildJobs: true is the default) unless 
          MaxBuildJobs: false is set.
        * InstallScript always disables UseMaxBuildJobs.

0.31.1 ""little white"" (2011-09-11)
        * Added support for Mac OS X 10.7.1.
        * Allow 32 bit systems to bootstrap on 10.6.
        * Simplified some code by taking advantage of the fact that the minimal
          supported OS version now is 10.5.
        * Bug fixes

0.31.0 "fib" (2011-07-20)
        * Added support for Mac OS X 10.7.
        * Dropped support for any Mac OS X version before 10.5. So 10.5, 10.6 and
          10.7 are the only supported OS X versions now.
        * Bug fixes

/-------------
| fink 0.30.x (see https://github.com/fink/fink/tree/branch_0_30)
\-------------

0.30.2 "Palin" (2011-07-11)
        * Last fink version for 10.4, and end of support for the OS.
        * Adds support for the 10.4-EOL subdirectory in dists.

0.30.1 "Hannity" (2011-06-28)

0.30.0 "Beck" (2011-04-30)

/-------------
| fink 0.29.x (see https://github.com/fink/fink/tree/branch_0_29)
\-------------

0.29.21 "Charter Oak" (2011-03-24)

0.29.20 "FirsTier" (2011-03-09)

0.29.19 "EarthStar" (2011-01-15)

0.29.18 "Darby" (2010-11-12)
        10.5/x86_64 only

0.29.17 "Tifton" (2010-11-11)

0.29.16 "K" (2010-11-09)

0.29.15 "Hillcrest" (2010-10-24)

0.29.14 "Bramble" (2010-10-19)

0.29.13 "Peninsula" (2010-07-01)

0.29.12 "TierOne" (2010-06-09)

0.29.11 "Greece and Portugal" (2010-06-02)

0.29.10 "Vantus" (2009-09-27)

0.29.9 "Dwelling House" (2009-08-28)

0.29.8 "Integrity" (2009-08-13)

0.29.7 "HBOS" (2009-06-10)

0.29.6 "New Frontier" (2009-05-20)

0.29.5 "Silverton" (2009-05-13)

0.29.4 (2009-05-12)
        again quickly replaced

0.29.3 (2009-05-12)
        quickly replaced

0.29.2 "IKB" (2009-04-14)

0.29.1 "Kaupthing" (2009-04-09)

0.29.0 "IndyMac" (2009-04-05)

/-------------
| fink 0.28.x (see https://github.com/fink/fink/tree/branch_0_28)
\-------------

New features:
        * Validate the shlibs field for consistency
        * Inclusion of .info file as a control file in the .deb
        * New selfupdate code to make future addition of methods easier
        * Automatic suggestion to run fink selfupdate if it hasn't been done in a while.
        * Remind user to selfupdate after enabling unstable
        * Display actual Distribution string in 'fink -V'
        * Use lftpget if available and appropriate
        * Private shared-library syntax in Shlibs

0.28.7 "Piltdown Man" (2009-02-19)

0.28.6 "The Philosopher's Stone" (2008-10-05)

0.28.5 "Spontaneous Generation" (2008-07-08)

0.28.4 "The Humors" (2008-06-29)

0.28.3 "Cold Fusion" (2008-06-20)

0.28.2 "N-ray" (2008-05-05)

0.28.1 "Phlogiston" (2008-03-11)

0.28.0 "Aether" (2008-01-20)

/-------------
| fink 0.27.x (see https://github.com/fink/fink/tree/branch_0_27)
\-------------

New features
        * fink --build-as-nobody tries to build as user fink-bld instead of nobody, which is reserved by the OS.
        * Timeouts for sluggish/stalled downloads.
        * Validator detects deficient checking of some script return codes in .info files.
        * New in 0.27.2, add conditionals support to Shlibs and ConfFiles field (requires using BuildDepends: fink (>= 0.27.2) or higher).

Bug fixes
        * Saner handling of virtual (Provides) packages directly from the fink command-line.
        * Better recovery when encountering an unprocessable .info file.
        * More reliable building perl-module packages (Type: perl passed -j1 in default InstallScript).
        * Improved detection of non-fink X11.
        * Safer management of communication between fink and apt-get.

0.27.16 "Defecaloesiophobia" (2008-07-08)

0.27.15 "Zemmiphobia" (2008-06-29)

0.27.14 "Liticaphobia" (2008-06-27)

0.27.13 "Triskaidekaphobia" (2008-06-22)

0.27.12 "Batrachophobia" (2008-06-20)

0.27.11 "Athazagoraphobia" (2008-02-17)

0.27.10 "Rhabdophobia" (2008-01-02)

0.27.9 "Paralipophobia" (2007-11-06)

0.27.8 "Ailurophobia" (2007-11-02)

0.27.7 "Potophobia" (2007-10-24)

0.27.6 "Hippopotomonstrosesquippedaliophobia" (2007-07-18)

0.27.5
        Never released to the public

0.27.4 "Kakorrhaphiophobia" (2007-07-10)

0.27.3 "Didaskaleinophobia" (2007-06-15)

0.27.2 "Blennophobia" (2007-06-10)

0.27.1 "Arachibutyrophobia" (2007-03-19)

0.27.0 "Gynophobia" (2007-03-17)

/-------------
| fink 0.26.x (see https://github.com/fink/fink/tree/branch_0_26)
\-------------

New features
        * Obsoletes support
        * Enable more than one Notify plugin at once
        * Type: -64bit, %lib, and %type_num[] (for building 64bit libs in parallel with 32bit libs)
        * new Distribution: field, which behaves like the Architecture: field
        * Change allowed filenames for .info file, to: invariant
          packagename, optionally followed by archname, optionally follwed by
          distribution, and finally optionally followed by either version or
          version-revision, each delimited by hyphens.
        * "fink configure" now allows to enable/disable the unstable tree
        * --dpkg-status and --all modes for fink cleanup
        * --tests mode to utilize InfoTest blocks
                * on Errors are fatal
                * warn Errors turn to warnings
        * --validate mode that causes packages to be validated
                * on Errors are fatal
                * warn Errors turn to warning
        * Info4 (added in 0.26.2)

0.26.4 "The Joy Luck Club" (2007-03-14)

0.26.3 "Divine Secrets of the Ya-Ya Sisterhood" (2007-03-08)

0.26.2 "Beaches" (2007-03-07)

0.26.1 "Thelma and Louise" (2007-01-22)

0.26.0 "Steel Magnolias" (2006-12-09)

/-------------
| fink 0.25.x (see https://github.com/fink/fink/tree/branch_0_25)
\-------------

New features
        * Incremental Indexing
        * SkipPrompts
                * Any more categories users would like?
        * Info3
                * Can indent nicely in .info files
                * No more support for RFC-822 multi-lines
                * Can put comments in pkglist fields
        * fast scanpackages with apt-ftparchive
        * auto-detection of country
        * Validator fixes:
                * detect InfoN property (should be wrapper)
        * New --trees option restricts fink to using .info files in the chosen tree(s).
        * new fink cleanup syntax
        * New --maintainer mode
        * New --log-output and --logfile flags to save transcripts of package building process
        * Integrated scanpackages, including ability to not index restrictive packages.
        * Support for running package test suites
        * reevaluate fink --tree=stable list
        * Validator:
                * Complain about > and < in dependency versioning (in .info).
                * dmacks: complete overhaul of .deb (val-unpack branch)
                * InfoN validator patch vasi fixed it the way he likes it
        * RangerRick: 'fink build foo-1.0-1' where a .deb exists in the bindist for foo-1.0-1 and UseBinaryDist is true should build locally, not fetch from the bindist.
        * Info3: allow comment lines in pkglist fields
        * "chown -h" functionality during --build-as-nobody (use Command:chowname_hr?)
        * dmacks: overhaul buildlocks to go away more automatically and have a cleaner cleanup
                * Automatically do cleanup when embarking on a package installation or removal
        * dmacks: buildlock destruction
                * Checking via lock_wait and PreRm
                * Removal on build failure via Fink::Finally
        * remove line-number in SysState error
        * BuildConflicts breakage
        * chown_hR is still leaving nobody-owned links.
        * progress bar during indexing ("." every 100 .info proces
