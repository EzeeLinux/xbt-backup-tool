# xbt-external_backup_tool
XBT -- External Backup Tool (Version 3.0)

1. Description:

 XBT is a program that makes keeping all of your user data safely backed up on
 a dedicated External USB drive easy. XBT works with Ubuntu 16.04 onward and
 the Linux Mint 18.x series and up. It also works with Debian 9 "Stretch" 
 and  distributions based on Debian like Linux Mint Debian Edition 3 "Cindy,"
 and MX Linux. 

2. Installation:

 Unaip the file `xbt_3.0.deb` and put it anywhere you wish. If you are working
 with a gra[hic desktop environment, simply drag on to the desktop and then
 double ckick it. Your distribution's deb package installer should open up and
 install it automatically.

 You can also install any deb package from a command line with these commands:

    sudo dpkg -i /path/to/deb/file followed by sudo apt-get install -f .

 --or--

    sudo apt install ./name.deb` (or /path/to/package/name.deb ). ...

 --or--

 Install gdebi, navaigate to the directory containing the deb file you wish to
 install and then run:

    sudo gdebi name.deb

 XBT will now be avaialble in your desktop menu.
 
3. Manual Installation:

 Copy the file 'xbt' to either to `/usr/local/bin` or `~/bin`, if you have a local
 bin folder setup. 

 The program is immediately available for use by running the command `xbt` in
 any terminal. XBT offers some direct terminal commands to jump to common
 functions. You can reead more about the in this file or in the only-line help
 page.

 Note: XBT won't work from a TTY or through SSH if the XBT Drive is not mounted
 at `/media/user-name/XBT_Drive`.

4. Un-installation

 You can un-install XBT simply by running this command:

    sudo apt remove xbt

 You can slo search for 'xbt' in your graphic software manager and choose to
 riomve it that way.

 Note: XBT only consists of three files

    xbt = automatically installed in /usr/bin
    xbt.desktop = automatically installed in /user/share/application
    xbt-icon.xpm = automatically installed in /usr/share/icons

 You can use any file search utility to look for these fiels if you want to
 remove them. XBT does not create any configuration files on the system.

 There is one called xbt-backup.log and that is placed on the dedicated
 XBT Drive.

5. License.

 XBT is free softare. You can redistribute it and/or modify it under the
 terms of the GNU General Public License Version 2.0. as published by
 the Free Software Foundation. A copy of the GNU GPL 2.0 is provided with the
 software.

6. Contents if Help Page:

 Commands:

 xbt = Starts XBT program with menu options.
 xbt --backup = Fully backs up host's /etc and /home directories to XBT_Drive.
 xbt --restore = Fully restores host machine's /home directory from XBT_Drive.
 xbt --help = Prints this help information.
 xbt --log = Prints log from XBT drive in interactive viewer. ("q" to exit.)

 Description:

 XBT is a program that makes keeping all of your user data safely backed up on
 a dedicated External USB drive.

 XBT will update files that have changed, remove files that have been
 deleted and add any new files that have been created since the last backup.
 The initial backup can take a lot of time if you have a lot of data stored
 in your system's /home directory. XBT creates a directory with the host name
 of the machine it's backing up from inside XBT-Backups. This allows users to
 share one XBT_Drive with multiple machines.

 The directory structure and all files are stored openly to allow users easy
 access if they only need to retrieve a few files or directories using a file
 manager. Data from /home can be restored with the built in "xbt restore"
 command if the user wants to roll back to the exact state of /home when the
 last backup was taken.

 A simple log file is added to the XBT_Drive that shows when each new
 backup is taken and any errors that might occur. This file is appended
 every time XBT is run. The log file is placed in XBT-Backups. You can view the
 last several backups by using the XBT Log viewer. Press "q" to exit when
 you're done.

 Requirements:

 XBT is designed to work with Ubuntu and Linux Mint but it should run
 on many other Linux distributions. You need to prepare an XBT Drive.
 This can be any USB storage device. The dedicated USB drive must be
 formatted to a Linux native file system such as Ext4 to ensure that file
 permissions will be stored unchanged. The USB drive needs to have enough
 free capacity to store all data in /home on all of the machines you want to
 use the drive for. The drive MUST be labeled as "XBT_Drive" for the script
 to run. If XBT_Drive is not detected, the script exits with an error.

 XBT Drive Setup allows you to choose a drive to designate as the XBT Drive. The
 selected drive will be "blanked," formatted with ext4 and labeled 'XBT_Drive."
 This option is available in the Main Menu.

 Feedback:

 Feel free to contact EzeeLinux with comments and suggestions for XBT and
 future projects.

 www.ezeelinux.com

 Enjoy using XBT!

 - Joe Collins

   December, 2017

 Disclaimer:

 THIS SOFTWARE IS PROVIDED BY EZEELINUX “AS IS” AND ANY EXPRESS OR IMPLIED
 WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
 MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO
 EVENT SHALL EZEELINUX BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
 EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR
 BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
 IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.

