# Cronie
Cronie contains the standard UNIX daemon crond that runs specified programs at
scheduled times and related tools. It is based on the original cron and
has security and configuration enhancements like the ability to use pam and
SELinux.

And why cronie? [http://www.urbandictionary.com/define.php?term=cronie]

# Download
Latest released version is 1.5.4.

User visible changes:

Release 1.5.4
- crond: Fix regression from previous release. Only first job from a crontab
  was being run.

Release 1.5.3
- Fix CVE-2019-9704 and CVE-2019-9705 to avoid local DoS of the crond.
- crontab: Make crontab without arguments fail.
- crond: In PAM configuration include system-auth instead of password-auth.
- crond: In the systemd service file restart crond if it fails.
- crond: Use the role from the crond context for system job contexts.
- Multiple small cleanups and fixes.

The source can be downloaded from [https://github.com/cronie-crond/cronie/releases]

Cronie is packaged by these distributions:
- Fedora [https://apps.fedoraproject.org/packages/cronie]
- Mandriva [http://sophie.zarb.org/srpm/Mandriva,cooker,/cronie/history]
- Gentoo [http://packages.gentoo.org/package/sys-process/cronie]
- Source Mage [http://dbg.download.sourcemage.org/grimoire/codex/stable/utils/cronie/]
- openSUSE [https://software.opensuse.org/package/cronie]
- Arch Linux [https://www.archlinux.org/packages/core/x86_64/cronie/]

# Contact

Mailing list: `cronie-devel AT lists.fedorahosted DOT org`

Bugs can be filled either into the issue tracker at this site or into [https://bugzilla.redhat.com/] Fedora product, component cronie. 
