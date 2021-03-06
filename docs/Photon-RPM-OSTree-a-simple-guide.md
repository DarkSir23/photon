Contents  
***

   [[Preface|Photon-RPM-OSTree:-Preface]]  

1. [[Introduction|Photon RPM-OSTree:-1-Introduction]]  
1.1 [[What is OSTree? How about RPM-OSTree?|Photon RPM-OSTree:-1-Introduction#11-what-is-ostree-how-about-rpm-ostree]]  
1.2 [[Why use RPM-OSTree in Photon?|Photon RPM-OSTree:-1-Introduction#12-why-use-rpm-ostree-in-photon]]  
1.3 [[Photon with RPM-OSTree installation profiles|Photon RPM-OSTree:-1-Introduction#13-photon-with-rpm-ostree-installation-profiles]]  
1.4 [[Terminology|Photon RPM-OSTree:-1-Introduction#14-terminology]]  
1.5 [[Sample code|Photon RPM-OSTree:-1-Introduction#15-sample-code]]  
1.6 [[How to read this book|Photon-RPM-OSTree:-1-Introduction#16-how-to-read-this-book]]  
1.7 [[RPM-OSTree in Photon OS 2.0|Photon-RPM-OSTree:-1-Introduction#17-rpm-ostree-in-photon-os-20]]  
2. [[Installing a Photon RPM-OSTree host against default server repository|Photon-RPM-OSTree:-2-Installing-a-host-against-default-server-repository]]  
2.1 [[Who is this for?|Photon-RPM-OSTree:-2-Installing-a-host-against-default-server-repository#21-who-is-this-for]]  
2.2 [[Installing the ISO, step by step|Photon-RPM-OSTree:-2-Installing-a-host-against-default-server-repository#22-installing-the-iso-step-by-step]]
3. [[Concepts in action|Photon-RPM-OStree:-3-Concepts-in-action]]  
3.1 [[Querying the deployed filetrees|Photon-RPM-OStree:-3-Concepts-in-action#31-querying-the-deployed-filetrees]]  
3.2 [[Bootable filetree version|Photon-RPM-OStree:-3-Concepts-in-action#32-bootable-filetree-version]]  
3.3 [[Commit ID|Photon-RPM-OStree:-3-Concepts-in-action#33-commit-id]]  
3.4 [[OSname|Photon-RPM-OStree:-3-Concepts-in-action#34-osname]]  
3.5 [[Refspec|Photon-RPM-OStree:-3-Concepts-in-action#35-refspec]]  
3.6 [[Deployments|Photon-RPM-OStree:-3-Concepts-in-action#36-deployments]]
4. [[Querying for commit, file and package metadata|Photon-RPM-OSTree:-4-Querying-for-commit,-file-and-package-metadata]]  
4.1 [[Commit history|Photon-RPM-OSTree:-4-Querying-for-commit,-file-and-package-metadata#41-commit-history]]  
4.2 [[Listing file mappings|Photon-RPM-OSTree:-4-Querying-for-commit,-file-and-package-metadata#42-listing-file-mappings]]  
4.3 [[Listing configuration changes|Photon-RPM-OSTree:-4-Querying-for-commit,-file-and-package-metadata#43-listing-configuration-changes]]  
4.4 [[Listing packages|Photon-RPM-OSTree:-4-Querying-for-commit,-file-and-package-metadata#44-listing-packages]]  
4.5 [[Querying for package details|Photon-RPM-OSTree:-4-Querying-for-commit,-file-and-package-metadata#45-querying-for-package-details]]  
4.6 [[Why am I unable to install, update or delete packages?|Photon-RPM-OSTree:-4-Querying-for-commit,-file-and-package-metadata#46-why-am-i-unable-to-install-update-or-delete-packages]]  
5. [[Host updating operations|Photon-RPM-OSTree:-5-Host-updating-operations]]  
5.1 [[Is it an update or an upgrade?|Photon-RPM-OSTree:-5-Host-updating-operations#51-is-it-an-update-or-an-upgrade]]  
5.2 [[Incremental upgrade|Photon-RPM-OSTree:-5-Host-updating-operations#52-incremental-upgrade]]  
5.3 [[Listing file differences|Photon-RPM-OSTree:-5-Host-updating-operations#52-listing-file-differences]]  
5.4 [[Listing package differences|Photon-RPM-OSTree:-5-Host-updating-operations#52-listing-package-differences]]  
5.5 [[Rollback|Photon-RPM-OSTree:-5-Host-updating-operations#55-rollback]]  
5.6 [[Deleting a deployed filetree|Photon-RPM-OSTree:-5-Host-updating-operations#56-deleting-a-deployed-filetree]]  
5.7 [[Version skipping upgrade|Photon-RPM-OSTree:-5-Host-updating-operations#57-version-skipping-upgrade]]  
5.8 [[Tracking parent commits|Photon-RPM-OSTree:-5-Host-updating-operations#58-tracking-parent-commits]]  
5.9 [[Resetting a branch to a previous commit|Photon-RPM-OSTree:-5-Host-updating-operations#59-resetting-a-branch-to-a-previous-commit]]  
6. [[Installing a Photon RPM-OSTree server|Photon-RPM-OSTree:-6-Installing-a-server]]  
7. [[Installing a Photon RPM-OStree host against a custom server repository|Photon-RPM-OSTree:-7-Installing-a-host-against-a-custom-server-repository]]  
7.1 [[Manual install of a custom host|Photon-RPM-OSTree:-7-Installing-a-host-against-a-custom-server-repository#71-manual-install-of-a-custom-host]]  
7.2 [[Automated install of a custom host via kickstart|Photon-RPM-OSTree:-7-Installing-a-host-against-a-custom-server-repository#72-automated-install-of-a-custom-host-via-kickstart]]  
8. [[File oriented server operations|Photon-RPM-OSTree:-8-File-oriented-server-operations]]  
8.1 [[Starting a fresh OSTree repo|Photon-RPM-OSTree:-8-File-oriented-server-operations#81-starting-a-fresh-ostree-repo]]  
8.2 [[Checking out a filetree|Photon-RPM-OSTree:-8-File-oriented-server-operations#82-checking-out-a-filetree]]  
8.3 [[Committing changes to a filetree|Photon-RPM-OSTree:-8-File-oriented-server-operations#83-committing-changes-to-a-filetree]]  
8.4 [[Downloading the changes at the host|Photon-RPM-OSTree:-8-File-oriented-server-operations#84-downloading-the-changes-at-the-host]]  
8.5 [[Creating summary metadata|Photon-RPM-OSTree:-8-File-oriented-server-operations#85-creating-summary-metadata]]  
9. [[Package oriented server operations|Photon-RPM-OSTree:-9-Package-oriented-server-operations]]  
9.1 [[JSON configuration file|Photon-RPM-OSTree:-9-Package-oriented-server-operations#91-json-configuration-file]]  
9.2 [[Package addition, removal, upgrade|Photon-RPM-OSTree:-9-Package-oriented-server-operations#92-package-addition-removal-upgrade]]  
9.3 [[RPMS repository|Photon-RPM-OSTree:-9-Package-oriented-server-operations#93-rpms-repository]]  
9.4 [[Composing a tree|Photon-RPM-OSTree:-9-Package-oriented-server-operations#94-composing-a-tree]]  
9.5 [[Automatic version prefix|Photon-RPM-OSTree:-9-Package-oriented-server-operations#95-automatic-version-prefix]]  
9.6 [[Installing package updates|Photon-RPM-OSTree:-9-Package-oriented-server-operations#96-installing-package-updates]]  
9.7 [[Creating server metadata|Photon-RPM-OSTree:-9-Package-oriented-server-operations#97-creating-server-metadata]]  
9.8 [[Starting a fresh OSTree repo|Photon-RPM-OSTree:-9-Package-oriented-server-operations#98-starting-a-fresh-ostree-repo]]  
10. [[Remotes|Photon RPM-OSTree:-10-Remotes]]  
10.1 [[Listing remotes|Photon-RPM-OSTree:-10-Remotes#101-listing-remotes]]  
10.2 [[GPG signature verification|Photon-RPM-OSTree:-10-Remotes#102-gpg-signature-verification]]  
10.3 [[Switching repositories|Photon-RPM-OSTree:-10-Remotes#103-switching-repositories]]  
10.4 [[Adding and removing remotes|Photon-RPM-OSTree:-10-Remotes#104-adding-and-removing-remotes]]  
10.5 [[List available branches|Photon-RPM-OSTree:-10-Remotes#105-list-available-branches]]  
11. [[Running container applications between bootable images|Photon-RPM-OSTree:-11-Running-container-applications-between-bootable-images]]  
11.1 [[Downloading a docker container appliance|Photon-RPM-OSTree:-11-Running-container-applications-between-bootable-images#111-downloading-a-docker-container-appliance]]  
11.2 [[Rebooting into an existing image|Photon-RPM-OSTree:-11-Running-container-applications-between-bootable-images#112-rebooting-into-an-existing-image]]  
11.3 [[Reboot into a newly created image|Photon-RPM-OSTree:-11-Running-container-applications-between-bootable-images#113-reboot-into-a-newly-created-image]]  
12. [[Install or rebase to Photon OS 2.0|Photon-RPM-OSTree:-Install-or-rebase-to-Photon-OS-2.0]]  
12.1 [[Installing an RPM-OSTree server|Photon-RPM-OSTree:-Install-or-rebase-to-Photon-OS-2.0#121-installing-an-rpm-ostree-server]]  
12.2 [[Installing an RPM-OSTree host|Photon-RPM-OSTree:-Install-or-rebase-to-Photon-OS-2.0#122-installing-an-rpm-ostree-host]]  
12.3 [[Rebasing a host from Photon 1.0 to 2.0|Photon-RPM-OSTree:-Install-or-rebase-to-Photon-OS-2.0#123-rebasing-a-host-from-photon-10-to-20]]  
12.4 [[Creating a host raw image|Photon-RPM-OSTree:-Install-or-rebase-to-Photon-OS-2.0#124-creating-a-host-raw-image]]    

[[Appendix A: Known issues|Photon-RPM-OSTree:-Appendix-A:-Known-issues]]  

***

About the author  
[Danut Moraru](mailto:dmoraru@vmware.com) is a Senior Software Design Engineer in the Photon OS Development team.  

[[Next page >|Photon-RPM-OSTree:-Preface]]