Command List Refernce for CSIA 295
==================================

Last updated 12/16/21
---------------------

### First Submission

---

**nmap** - a utility used for scanning networks and hosts for open services/ports on external or internal networks. *nmap [Options] [Target...]*

**arp-scan** - *arp-scan [options] hosts..*. - arp-scan sends arp packets out on the local network and returns any responses from hosts on the network that are received.

**tail** - returns the last 10 lines of output from a command or file by default, can be changed by specifying the number of lines to return. tail *[OPTION]... [FILE]...*

**zenmap** - the GUI front-end for the nmap network utility. *zenmap [ <options> ] [ <results file> ]*

**more** - Linux/Unix command to read content of a file. *more [-options] [-num] [+/pattern] [+linenum] [file_name]*

**grep** - Linux/Unix command to search through the output read from a command. *grep [options] pattern [files]*

**net** - Windows command used to configure or view network settings. *net [accounts | computer | config | continue | file | group | help | helpmsg | localgroup | name | pause | print | send | session | share | start | statistics | stop | time | use | user | view]*

**gpedit.msc** - command to use at the command prompt to open the group policy editor in Windows.

---

### Second Submisison

**ifconfig** - used to manage network configuration on unix/linux systems and query network interfaces. This is now deprecated and has been replaced with the ip command in most systems.

**nbstat** - Windows command used to query NetBIOS name over TCP/IP protocol stats. Can prob both local and remote machines. *nbtstat [/a <remotename>] [/A <IPaddress>] [/c] [/n] [/r] [/R] [/RR] [/s] [/S] [<interval>]*

**cat** - linux/unix command used to read/output files. Output can be piped or redirected to new file (cat file > newfile) or append file (cat file >> file).

**cp** - linux/unix command to copy files. *cp [originalFile] [newFileName]*

**route** - linux/unix command to manipulate and display routing table. route by itself will display the routing table of the machine where the command is being issued. **deprecated**; *use ip route on modern distros*. 
[https://www.redhat.com/sysadmin/route-ip-route](https://www.redhat.com/sysadmin/route-ip-route)

**echo** - linux/unix command to output strings passed as arguments, can be redirected to file or can be used to call shell variables 

**service** - linux/unix command used to start System V init script types services. Example: service httpd start. *deprecated on systemd init type systems, replaced with systemctl*

**msfconsole** - command to start metasploit from the command line

**db_nmap** - used in metasploit to store the nmap results in the database

**hosts** - in metasploit this is used to display all the discovered hosts

**whoami** - linux/unix command to output the current user

**clear** - linux/unix command to clear output from the terminal window

**banner** - in metasploit, used to get a different banner

**search** - in metasploit, used to search for modules

**use** - in metasploit, used to select a module

**info** - in metasploit, after selecting module to get information on module

**set** - in metasploit, used to set options in module

**show options** - in metasploit, used to show the current options

**run** - in metasploit, run the module selected

**mysql** - run mysql from the command line. *mysql -u [username] -h[hostname,ipaddress] -p [password]*

**show databases; - display databases in mysql

**use [databasename];** - select the database in mysql

**show tables;** - display the tables from the selected database in mysql

**select * from [tableName]l** - shows all records from the table selected in mysql.

**netstat** - linux/unix/windows. displays active tcp connections, ports on which the computer is listening. Windows: *netstat [-a] [-b] [-e] [-n] [-o] [-p <Protocol>] [-r] [-s] [<interval>]*
In some linux distros, has been deprecated in favor of the *ss* command. [https://www.redhat.com/sysadmin/netstat](https://www.redhat.com/sysadmin/netstat)

---

### Final Submission

**tcpdump** - a Unix/Linux command line tool used for analyzing captured packets. *tcpdump [ -AbdDefhHIJKlLnNOpqStuUvxX# ] [ -B buffer_size ] [ -c count ] [ -C file_size ] [ -G rotate_seconds ] [ -F file ] [ -i interface ] [ -j tstamp_type ] [ -m module ] [ -M secret ] [ --number ] [ -Q in|out|inout ] [ -r file ] [ -V file ] [ -s snaplen ] [ -T type ] [ -w file ] [ -W filecount ] [ -E spi@ipaddr algo:secret,...  ] [ -y datalinktype ] [ -z postrotate-command ] [ -Z user ] [ --time-stamp-precision=tstamp_precision ] [ --immediate-mode ] [ --version ] [ expression ]*

**capinfos** - Provided by Wireshark and used at the command line. Prints information about capture files. Usage: *capinfos [ -a ] [ -A ] [ -b ] [ -B ] [ -c ] [ -C ] [ -d ] [ -D ] [ -e ] [ -E ] [ -F ] [ -h ] [ -H ] [ -i ] [ -I ] [ -k ] [ -K ] [ -l ] [ -L ] [ -m ] [ -M ] [ -n ] [ -N ] [ -o ] [ -q ] [ -Q ] [ -r ] [ -R ] [ -s ] [ -S ] [ -t ] [ -T ] [ -u ] [ -v ] [ -x ] [ -y ] [ -z ] <infile>*

**iwconfig** - used in Linux to configure wireless networks and connections, similar to ifconfig for wired connections. *Deprecated in some distros of Linux and replaced with the iw command* Usage: *iwconfig [interface] iwconfig interface [essid X] [nwid N] [mode M] [freq F] [channel C][sens S ][ap A ][nick NN ] [rate R] [rts RT] [frag FT] [txpower T] [enc E] [key K] [power P] [retry R] [modu M] [commit] iwconfig --help iwconfig --version*

**airmon-ng** - This script can be used to enable monitor mode on wireless interfaces. It may also be used to go back from monitor mode to managed mode. Entering the airmon-ng command without parameters will show the interfaces status. Usage: *airmon-ng <start|stop> <interface> [channel] or airmon-ng <check|check kill>*

**aircack-ng** - Aircrack-ng is a complete suite of tools to assess WiFi network security. Used to attack clients rather than the wireless access point. Usage: *airbase-ng <options> <replay interface>* See [https://www.aircrack-ng.org/doku.php?id=airbase-ng](https://www.aircrack-ng.org/doku.php?id=airbase-ng) for options.

**airdecap-ng** - With airdecap-ng you can decrypt WEP/WPA/WPA2 capture files. As well, it can also be used to strip the wireless headers from an unencrypted wireless capture. It outputs a new file ending with "-dec.cap" which is the decrypted/stripped version of the input file. Usage: *airdecap-ng [options] <pcap file>* See [https://www.aircrack-ng.org/doku.php?id=airdecap-ng](https://www.aircrack-ng.org/doku.php?id=airdecap-ng) for more options.

**ntdsutil** - Windows command line utility tool for interacting with Active Directory services. Can be used to create a back-up of the Active Directory database file, ntds.dit. Usage: *Ntdsutil [activate instance %s | authoritative restore | change service account %s1 %s2 | configurable settings | DS behavior | files | group membership evaluation | Help | ifm | ldap policies | ldap port %d | list instance | local roles | metadata cleanup | partition management | popups on | popups off | quit | roles | security account management | semantic database analysis | set DSRM password | snapshot | SSL port %d]*

**python3-impacket** - Impacket is a collection of Python3 classes focused on providing access to network packets. Impacket allows Python3 developers to craft and decode network packets in simple and consistent manner. It includes support for low-level protocols such as IP, UDP and TCP, as well as higher-level protocols such as NMB and SMB. Secrets dump usage: *impacket-secretsdump [-h] [-ts] [-debug] [-system SYSTEM] [-bootkey BOOTKEY] [-security SECURITY] [-sam SAM] [-ntds NTDS] [-resumefile RESUMEFILE] [-outputfile OUTPUTFILE] [-use-vss] [-exec-method [{smbexec,wmiexec,mmcexec}]] [-just-dc-user USERNAME] [-just-dc] [-just-dc-ntlm] [-pwd-last-set] [-user-status] [-history] [-hashes LMHASH:NTHASH] [-no-pass] [-k] [-aesKey hex key] [-keytab KEYTAB] [-dc-ip ip address] [-target-ip ip address] target*

**john** - John the Ripper is an Open Source password security auditing and password recovery tool available for many operating systems. Usage: *john [OPTIONS] [PASSWORD-FILES]* See [https://www.kali.org/tools/john/](https://www.kali.org/tools/john/) for further options.

**dsquery** - Used in Windows from the command prompt to query Active Directory by using search criteria that you specify. Each of the dsquery commands finds objects of a specific object type, with the exception of dsquery *, which can query for any type of object. Usage: *dsquery * [{<StartNode> | forestroot | domainroot}] [-scope {subtree | onelevel | base}] [-filter <LDAPFilter>] [-attr {<AttributeList> | *}] [-attrsonly] [-l][{-s <Server> | -d <Domain>}] [-u <UserName>] [-p {<Password> | *}] [-q] [-r] [-gc] [-limit <NumberOfObjects>] [{-uc | -uco | -uci}]*

**dsmod** - Used in Windows from the command prompt to manipulate entries in Active Directory. Can make modifications to an existing object of a specific type in the directory, such as users and groups. See [https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/cc732406(v=ws.11)](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/cc732406(v=ws.11)) for full reference. Usage for updating a user object: *dsmod user <UserDN> ... [-upn <UPN>] [-fn <FirstName>] [-mi <Initial>] [-ln <LastName>] [-display <DisplayName>] [-empid <EmployeeID>] [-pwd (<Password> | *)] [-desc <Description>] [-office <Office>] [-tel <PhoneNumber>] [-email <E-mailAddress>] [-hometel <HomePhoneNumber>] [-pager <PagerNumber>] [-mobile <CellPhoneNumber>] [-fax <FaxNumber>] [-iptel <IPPhoneNumber>] [-webpg <WebPage>] [-title <Title>] [-dept <Department>] [-company <Company>] [-mgr <Manager>] [-hmdir <HomeDirectory>] [-hmdrv <DriveLetter>:] [-profile <ProfilePath>] [-loscr <ScriptPath>] [-mustchpwd {yes | no}] [-canchpwd {yes | no}] [-reversiblepwd {yes | no}] [-pwdneverexpires {yes | no}] [-acctexpires <NumberOfDays>] [-disabled {yes | no}] [{-s <Server> | -d <Domain>}] [-u <UserName>] [-p {<Password> | *}][-c] [-q] [{-uc | -uco | -uci}]* 