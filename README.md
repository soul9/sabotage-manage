Sabotage-manage, a set of scripts to simplify building and maintenance of sabotage filesystems
==============================================================================================

Projects live in the projects directory, in any subdirectory. I use the projects/$target_arch/$project_name structure, but this can change.

This is work in progress, but the usage is:

    sudo bin/buildhost "projectname"
    sudo bin/buildtarget "projectname"

To enter a chroot for a project

    sudo bin/enter_chroot "projectname" "host|target"

If you enter in target mode, the target rootfs will be mounted inside the host one.

There are some scripts there to help with saving and restoring chroots, but that remains mostly TODO.