WinNFSd is a Network File System (NFS) server for Windows. 
You can use any NFS client to mount a directory of Windows
and read/write files via NFS protocol. 
It is useful when you usually access files of Windows on Linux.

[Usage]
	winnfsd.exe [-id <uid> <gid>] [-log on | off] <export path>
	uid: The user id of the directory and all files under this directory, used by the client.  Default is 0 (uid of root).
	gid: The group id of the directory and all files under this directory, used by the client.  Default is 0 (gid of root).
	log: If on, WinNFSd will print messages.  Default is on.
	export path: The path on Windows which you want to export.  The client can read/write files under this path.
	             For example, C:\work\cpp.  The client must mount it using /C/work/cpp.


[History]
	2005/9/13 v2.0
		+ Support NFS version 3 (RFC 1813)
		+ Add some commands in user interface.
		+ Improve performance.

	2005/5/9 v1.0
		+ Support RPC version 2 (RFC 1057) and NFS version 2 (RFC 1094)
		+ Command-mode interactive user interface.
		+ Warn if there are clients still mount when you quit the server.


[Contact]
	vincent0629@gmail.com
