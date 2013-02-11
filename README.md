CSU-CSB-Room-Lookup
===================

 Look up who is currently logged-in to the machines of a given room in the CSU CS Building.
 
 Help-Text Output:
## # # # # # # # # # # # #
## CS Room Lookup Script #
## # # # # # # # # # # # #
##  Look up who is currently logged-in to the machines of a given room
##     in the CS Building.
##
##  If multiple users are connected, the script will attempt to choose
##     the user who is most likely the one currently sitting at that
##     machine.
##
## Valid Room IDs #
### # # # # # # # #
##           Room -- RoomID
##   CSB Room 120 --  120 (default is your current room)
##   CSB Room 215 --  215
##   CSB Room 225 --  225
##
## Valid Output Types #
### # # # # # # # # # #
##              Type -- OutputType
##  Last, First Name -- (n)ames (default)
##          Username -- (u)sers
##      Machine Name -- (m)achines
##
## Script Usages #
## # # # # # # # #
##   ~$ ~/lookup RoomID
##   ~$ ~/lookup RoomID OutputType
##   ~$ ~/lookup RoomID OutputType > FileNameToStoreChart.txt
##
## Using the lookup scripts' internal functions #
### # # # # # # # # # # # # # # # # # # # # # # #
##   ~$ source ~/lookup
##

 Sourcing Output:
## CS Room Lookup Script (Sourced) ##
# Lookup Script Functions:
 ~$ whoisat - Returns the username of a user at a given machine, if any
       Usage: whoisat <machine-name>[TAB to AutoComplete]
 ~$ getname - Returns the Last, First Name from a given username
       Usage: getname <user-name>
 ~$ whereami - Returns the machine-name of the machine you are at
       Usage: whereami
 ~$ gna - Returns a (formatted) Last, First Name of the user at a given machine, if any (helper function)
       Usage: gna <machine-name>[TAB to AutoComplete]

2/10/2013
